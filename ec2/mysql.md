#Mysql 設定


##mysql 安裝
```
sudo apt-get update
sudo apt-get install mysql-server mysql-client
```
 
##mysql config 設定

```
sudo vim /etc/mysql/my.cnf
``` 

##my.conf 修改
```
//讓所有ip都可以連
bind_address = 0.0.0.0
```

##開啟mysql
```
sudo service mysql start
```

##登入msql 
```
mysql -u root -p
```
##測試看看有沒有成功

##如果要從外部遠端連線進來就必須要到AWSEC2的控制台在Security Groups中找到機器對應的項目中到Inbound中編輯開啟port
 
