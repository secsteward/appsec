# appsec
something about appsec

# 解决BurpSuite测试手机APP的时候，一些走HTTPS协议的包总是会响应很慢的问题：
思路：Browser -> Fiddler -> BurpSuite


1.配置Fiddler
Tools -> Options -> Gateway， 填入：http://127.0.0.1:8080;https://127.0.0.1:8080
将BurpSuite设置为Fiddler的代理， 这样Fiddler流量将会发往BurpSuite。


2.配置手机
Fiddler需要在手机端安装证书。
Fiddler的默认监听端口为8888，将手机监听的端口改为8888即可。
