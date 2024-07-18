# step 1 : install java pada Linux  
```
sudo apt install default-jdk
```
# step 2 : install mysql-connector 
```
wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-j_9.0.0-1ubuntu24.04_all.deb
```
# step 3 : karena ini format nya adalah deb silahkan ekstrak .deb tersebut dengan perintah : 
```
sudo dpkg -i path/to/mysql-connector-j_9.0.0-1ubuntu24.04_all.deb
```
# step 4 : setelah itu periksa apakah MySQL connector benar benar ada atau tidak : 
```
ls /usr/share/java | grep mysql-connector
```
# step 5 : silahkan jika benar benar sudah di install java MySQL connector nya langsung compile file java tersebut : 
```
javac -cp .:/usr/share/java/mysql-connector-java-9.0.0.jar(MySQL connector nya tergantung versi nya) userCRUD.java
```
# step 6 compile program tersebut  : 
```
java -cp .:/usr/share/java/mysql-connector-java-9.0.0.jar UserCRUD
```

Happy codinggg !!!!!