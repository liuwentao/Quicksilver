# 爬虫计划


## 安装

安装 pip

```shell
$ curl "https://bootstrap.pypa.io/get-pip.py" -o "get-pip.py"
$ sudo python get-pip.py
$ rm get-pip.py
```

安装 podgen

```shell
$ sudo pip install podgen
$ sudo pip install requests
$ sudo pip install lxml 或者 sudo apt-get install python-lxml
$ sudo pip install beautifulsoup4
```

或者使用 virtualenv

```shell
$ sudo pip install virtualenv
$ sudo virtualenv --no-site-packages podcast --always-copy
$ pip install -r requirements.txt
$ deactivate # 退出虚拟环境
```

## 使用

单个专辑

```shell
$ python app.py ximalaya 8475135 # 喜马拉雅
$ python app.py qingting 212192  # 蜻蜓fm
```

多个专辑，参数使用英文逗号

```shell
$ python app.py xiamalaya 8475135,269179
```

[目前已经支持的节目单](https://github.com/forecho/Quicksilver/wiki/%E7%9B%AE%E5%89%8D%E5%B7%B2%E7%BB%8F%E6%94%AF%E6%8C%81%E7%9A%84%E8%8A%82%E7%9B%AE%E5%88%97%E8%A1%A8)，目前此脚本只支持喜马拉雅的专辑转换为 RSS，如果需要更多节目，欢迎提交 [Issues](https://github.com/forecho/Quicksilver/issues)。
