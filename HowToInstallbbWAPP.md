How To Install bWAPP in ubuntu Server

1. Download files bWAPP_latest.zip
2. extract file :
   unzip bWAPP_latest.zip
3. copy or move file bWAPP to /var/www/html :
   mv bWAPP_latest/bWAPP /var/www/html/
4. Give access permissions to the folder :
   chmod -R 777 /var/www/html/bWAPP
5. Open folder bWAPP and give permissions to folder images/ and passwords/
   chmod 777 images/
   chmod 777 passwords/
6. edit file settings.php
   nano /bWAPP/admin/settings.php
   and change the setting follow :
   $db_server     ="localhost"
   $db_username   ="root"
   $db_password   ="toor" ("if mysql using a password, and if it should not be a [""])
   $db_name       ="bWAPP"
   exit : ctrl + c
7. run apache2 and mysql :
   /etc/init.d/apache2 start
   /etc/init.d/mysql start
8. open your browser, and when the ip
   of ubuntu server, example :
   192.168.1.102/bWAPP/install.php
9. i think you already know the next process :D
