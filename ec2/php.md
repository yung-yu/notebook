#PHP安裝

##安裝指令
```
sudo apt-get update
sudo apt-get install php5 libapache2-mod-php5
```
##到你的DocumentRoot裡
```
echo "<?php phpinfo();?>" > phpinfo.php
```
##開啟瀏覽器
```
http://your_ip/phpinfo.php
```