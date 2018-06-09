# -SL-TGN-Gate-Network

Tested on Apache2 with php5


Replace fcgid.conf in:etc/apache2/mods-available/

Open liberay/lib.php
enter your mysql db login in this section (at line 29):
if($db_name == "stargate_t")
  {
    $dbname="XXXXXXXXXX";
    $dbhost="localhost";
    $dbuser="XXXXXXXXXX";
    $dbpass="XXXXXXXXXX";
    mysql_connect($dbhost,$dbuser,$dbpass);
    mysql_select_db($dbname);
  }

Open intsall.php with browser for install mysql db table.
Import gate_50.sql to mysql database

Open all lsl-scripts and change the URL in the first lines to your server.
