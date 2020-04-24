# 基于python的网路磁盘系统 (Ant Disk)

Ant Disk是一个仿百度云盘布局的一个云盘系统，它支持web端和pc端，代码性能和质量还有待改进，目前是把功能实现

## 特点
- 同一份文件在系统中只有一份，通过md5来作为唯一标识，以此来节省服务器磁盘
- 支持断电续传

## 基础功能
 - 用户登录
 - 用户注册
 - 显示用户目录列表
 - 对文件进行预览（查看图片， 查看pdf文件）
 - 下载文件
 - 上传文件
 - 分类显示文件（如图片，文档）
 - 分享文件（生成分享链接，下载他人分享文件， 添加他人分享文件到自己的目录中）


## 开始

克隆项目到你的磁盘中

在安装完必须的python包后，请先把user_folder文件清空，并创建数据库disk，在config.py编辑连接数据库配置

### 数据库迁移
python manage.py db init
python manage.py db migrate
python manage.py db upgrade

### 运行程序
python manage.py runserver -h 0.0.0.0 -p 12345


## 目录

├─`app` 代码  
├─`file_data` 文件数据  
├─`user_folder` 用户的个人目录 



