# 《Django Web框架教学笔记》
### 目录
[TOC]

- 课程特点：
    1. 学习难度大，大部分内容需要理解并记忆
    2. 文件较多易混淆
    3. 学习阶段注重框架使用，工作阶段注重实现业务逻辑
    4. 综合应用强，小练习少

## Django框架的介绍
- 2005年发布,采用Python语言编写的开源web框架
- 早期的时候Django主做新闻和内容管理的
- 一个重量级的 Python Web框架，Django 配备了常用的大部分组件
    1. 基本配置
    1. 路由系统
    1. 原生HTML模板系统
    1. 视图 view
    1. Model模型,数据库连接和ORM数据库管理
    1. 中间件
    1. Cookie & Seesion
    1. 分页
    1. 数据库后台管理系统admin

- Django的用途
    - 网站后端开发
    - 微信公众号、微信小程序等后台开发
    - 基于HTTP/HTTPS协议的后台服务器开发
        - 在线语音/图像识别服务器
        - 在线第三方身份验证服务器等
    
- Django的版本
    - 最新版本:2.2.x
    - 当前教学版本:1.11.8

- Django的官网
    - 官方网址: <http://www.djangoproject.com>
    - 中文文档(第三方):
        - <https://yiyibooks.cn/>
        - <http://djangobook.py3k.cn/>
    - Django的离线文档
        1. 解压缩数据包 `django-docs-1.11-en.zip`
        2. 用浏览器打开 `django-docs-1.11-en/index.html`


### Django的安装
- 查看已安装的版本
    ```python
    >>> import django
    >>> print(django.VERSION)
    (1, 11, 8, 'final', 0)
    ```
- 安装
    1. 在线安装
        - `sudo pip3 install django`  安装django的最新版本
        - 或
        - `sudo pip3 install django[==版本]` 安装django的指定版本
        - 如:
            - `sudo pip3 install django==1.11.8`
    2. 离线安装
        - 下载安装包:
        - 安装离线包
            - `tar -xvf Django-1.11.8.tar.gz`
            - `cd Django-1.11.8`
            - `sudo python3 setup.py install`
    3. 用wheel离线安装
        - 下载安装包:
            - `pip3 download -d /home/tarena/django_packs django==1.11.8`
        - 安装离线包
          - `pip3 install Django-1.11.8.whl`
- Django的卸载
  
- `pip3 uninstall django`
  
- Django 的开发环境
    - Django 1.11.x 支持 Python 2.7, 3.4, 3.5 和 3.6（长期支持版本 LTS)
    - 注: Django 1.11.x 不支持 Python 3.7
