#Apache confing 設定

###將原本的000-default.conf複製一份my.conf來編緝.
```
 sudo cp /etc/apache2/sites-available/000-default.conf /etc/apache2/sites-available/my.conf
```   
###編輯my.conf
```
 sudo vim etc/apache2/sites-available/my.conf
```
###my.conf內容
```
<VirtualHost *:80>
  ServerAdmin yungyu405728@gmail.com

  DocumentRoot /home/ubuntu/www/

  ErrorLog ${APACHE_LOG_DIR}/error.log
  CustomLog ${APACHE_LOG_DIR}/access.log combined

  <Directory /home/ubuntu/www/ >
 AllowOverride All
      Require all granted
      Allow from all
</Directory>
</VirtualHost>
```
### 將my.conf設定 sites-enabled
```
sudo a2ensite my.conf
```  
###如果在sites-enabled還有其他conf記得刪掉
```
sudo a2dissite 000-default.conf
```
###最後將apache重啟
```
sudo services apache2 restart
```