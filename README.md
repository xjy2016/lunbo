# lunbo
- 测试：在bin目录下
mongod.exe --dbpath="D:\Program Files\MongoDB\data\db"
- 此条命令可以百发百中：
- 在bin目录下，并且是管理员命令行
mongod.exe --bind_ip 127.0.0.1 --logpath "D:\Program Files\MongoDB\data\logs\logs.log" --logappend --dbpath "D:\Program Files\MongoDB\data\db" --port 20000 --serviceName "MongoDB" --serviceDisplayName "MongoDB" --install
- 原命令：
mongod.exe --bind_ip yourIPadress --logpath "C:\data\dbConf\mongodb.log" --logappend --dbpath "C:\data\db" --port yourPortNumber --serviceName "YourServiceName" --serviceDisplayName "YourServiceName" --install


* --bind_ip		绑定服务IP，若绑定127.0.0.1，则只能本机访问，不指定默认本地所有IP
* --logpath		定MongoDB日志文件，注意是指定文件不是目录
* --logappend		使用追加的方式写日志
* --dbpath		指定数据库路径
* --port			指定服务端口号，默认端口27017
* --serviceName		指定服务名称
* --serviceDisplayName	指定服务名称，有多个mongodb服务时执行。
* --install		指定作为一个Windows服务安装。
