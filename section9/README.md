## 网络异常处理

#####1.网络掉线

* 要求服务器监测到掉线一端存储数据到客户端: PleaseSaveClass  (服务器主动发起)

>服务端发起请求:

> * 如果有客服端掉线发送给另外一端

>```javascript
    result : {}
 ```
 data: 数据为空

> 客户端处理:
 * 存储课程数据到服务器并等待另外一端上线 (发送 reqSaveClass)

* 系统初始化完毕: InitOK

>客户端请求格式:
 ```javascript
    data : {}
 ```
 服务端处理:
 * 将数据原封不动转发给另一客户端

>```javascript
     result : {}
  ```
 data: 数据为空
