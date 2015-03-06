## 聊天框部分

##### 1.聊天消息
* 聊天消息转发 : ChatMessages

>客户端请求格式:
 ```javascript
    data : {
        own: "xxx", // 发送人 类型
        msg: "xxx"  // 发送消息
    }
 ```
  服务端处理:
  * 将数据原封不动转发给另一客户端

>```javascript
    result : {
        own: "xxx", // 发送人 类型
        msg: "xxx"  // 发送消息
    }
 ```
 data : 聊天数据