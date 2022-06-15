
TryHackMe_Gallery
===================

if(!defined('base_url')) define('base_url',"http://" . $_SERVER['SERVER_ADDR'] . "/gallery/");

if(!defined('base_app')) define('base_app', str_replace('\\','/',__DIR__).'/' );

if(!defined('dev_data')) define('dev_data',$dev_data);

if(!defined('DB_SERVER')) define('DB_SERVER',"localhost");

if(!defined('DB_USERNAME')) define('DB_USERNAME',"gallery_user");

if(!defined('DB_PASSWORD')) define('DB_PASSWORD',"passw0rd321");

if(!defined('DB_NAME')) define('DB_NAME',"gallery_db");

mysql --user= gallery_user --password=passw0rd321 gallery_db

b3stpassw0rdbr0xx
