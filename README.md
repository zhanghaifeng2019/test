# 本システムについて
## 開発を始める前に
  1. 下記の環境固有の変数を埋めてください。  
  - application/config/development/config.php （ℓ73-74）  

  ```php:application/config/development/config.php  
  $config['base_url'] = '【開発用のベースURL】';
  ```  
※必ずURLの末尾に「/」を入れないこと！
例）http:/dev.weekly.kenki-shimpou.com

  -  application/config/development/database.php （ℓ73-74）  

  ```php:application/config/development/database.php  
  $db['default'] = array(
    'dsn'   => 'mysql:host=localhost;port=3306;dbname=kenki-shimpou',
    'username' => '【DBのユーザ名】',
    'password' => '【DBのパスワード】',
    'dbdriver' => 'pdo',
    'dbprefix' => '',
    'pconnect' => FALSE,
    'db_debug' => (ENVIRONMENT !== 'production'),
    'cache_on' => FALSE,
    'cachedir' => '',
    'char_set' => 'utf8',
    'dbcollat' => 'utf8_general_ci',
    'swap_pre' => '',
    'encrypt' => FALSE,
    'compress' => FALSE,
    'stricton' => FALSE,
    'failover' => array(),
    'save_queries' => TRUE
  );
  ```
