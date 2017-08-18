# openssl-auto-ca
openssl使用配置文件生成server和client证书

# 使用
直接运行脚本,即可得到相关证书.


    $./createcert.sh


生成的目录类似如下:

    zhaofeng@zhaofeng-pc:~/Git/bootstrap/openssl-auto-ca$ tree
    .
    ├── createcert.sh
    ├── myca
    │   ├── client
    │   │   ├── cert.pem
    │   │   ├── keycert.p12
    │   │   ├── key.pem
    │   │   └── req.pem
    │   ├── root
    │   │   ├── cacert.cer
    │   │   ├── cacert.pem
    │   │   ├── certs
    │   │   │   ├── 01.pem
    │   │   │   └── 02.pem
    │   │   ├── index.txt
    │   │   ├── index.txt.attr
    │   │   ├── index.txt.attr.old
    │   │   ├── index.txt.old
    │   │   ├── private
    │   │   │   └── cakey.pem
    │   │   ├── serial
    │   │   └── serial.old
    │   └── server
    │       ├── cert.pem
    │       ├── keycert.p12
    │       ├── key.pem
    │       └── req.pem
    └── openssl.cnf

    6 directories, 21 files

# 修改参数
直接修改`createcert.sh`文件的用户自定义部分内容,然后重新执行,生成新的证书.
 
