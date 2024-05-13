# 胡扯
套接字通信部分借鉴了[这个项目](https://github.com/techwithtim/Python-Live-Chat-App)，然后其他的基本就是乱搞，有的页面借鉴了一些赛题😋
#  部署
## 直接部署
修改app.py中数据库连接部分，改为你自己的数据库信息，然后直接运行app.py，最后访问
```
http://localhost:5000
```
## docker 部署
```
docker-compose -p crypto up --build -d
```
或
```
docker-compose up --build -d
```
# 预览
## 首页
![](.\img\图片1.png)
## 登录
![2](.\img\图片2.png)

## 注册
![](.\img\图片3.png)
## 登陆后聊天主页
![](.\img\图片4.png)
## 聊天室
![](.\img\图片5.png)
## 网站日志
![](.\img\图片7.png)
## 日志查看—创建房间
![](.\img\图片8.png)
## 日志查看—另一用户加入房间并完成密钥协商
因为容器化了，这个函数又是在另一个文件，所以只想到将输出信息设置到一个日志文件中，然后进入容器化交互查看这种查看方法
![](.\img\图片9.png)
## 日志查看—发送消息中间量
![](.\img\图片10.png)