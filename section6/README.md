## 上传图片部分

#####1.获取存储服务器认证Token码

* 获取存储服务器认证Token码 : UpLoadToken

>客户端请求格式:
 ```javascript
    data : {}
 ```
 data: 数据为空

> 服务端处理:
  * 发送存储服务器认证Token码到请求端

>```javascript
    result : {
        token: "xxx"
    }
 ```
 data: 存储服务器认证Token码