collipa
=======
## 简介

The source of <http://collipa.com>

## 配置

```
mv config.back.py config.py
```
修改 collipa/config.py 文件：

### 数据库

- _DBUSER = "username" # 数据库用户名
- _DBPASS = "password" # 数据库密码
- _DBHOST = "localhost" # 数据库地址
- _DBNAME = "collipa" # 数据库名称

### 邮箱

- _SMTPUSER = 'example@gmail.com' # 邮箱用户名
- _SMTPPASS = 'password' # 邮箱密码
- _SMTPHOST = 'smtp.gmail.com' # 邮箱地址
- _SMTPPORT = '587' # 邮箱端口

### secret

- cookie_secret = 'cookiesecret' # cookie secret 随机字符
- password_secret = 'passwordsecret' # password secret 随机字符

## 安装必要扩展包

### 安装 lamp包

```
sudo apt-get install lamp-server^
```

### ubuntu需要安装的其他程序
```
sudo apt-get install memcached redis-server libtiff5-dev libjpeg8-dev zlib1g-dev libfreetype6-dev liblcms2-dev libwebp-dev tcl8.6-dev tk8.6-dev python-tk python-dev libmysqlclient-dev     

```

### 安装其他

```
sudo pip install -r requirements.txt  -i http://pypi.douban.com/simple/ 
```

## 初始化数据库

```
python setup.py --init
```

## 运行

```
python manage.py app runserver
```

##License

Released under the WTFPL license:

http://www.wtfpl.net
