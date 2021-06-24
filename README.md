### 这是一个基于python+flask+sqlalchemy的课程，学生，老师信息管理系统
* ****
### 1.安装相关依赖性
```bash
pip3 install -r ./requirements.txt
```
### 2.初始化数据库
``` bash
python ./manage.py db init
```
### 3.数据库迁移
```bash
python ./manage.py db migrate
```
### 4.数据库升级
```bash
python ./manage.py db upgrade
```
### 5.导入虚拟数据
```bash
python ./manage.py generate_fake
```
### 6.启动web服务
```bash
python ./manage.py runserver
```
## Q&A
### Q1. 所用数据库
```
# 为了方便运行，默认采用了sqlite，如果想用别的数据库，请自信导入环境变量
SQLALCHEMY_DATABASE_URI = os.environ.get('DEV_DATABASE_URL') or \
                        'sqlite:///' + os.path.join(basedir, 'db.sqlite')
```
## Reference
[WolfMy/course_select_system](https://github.com/WolfMy/course_select_system) 