## 数据持久化处理部分

#####1.保存每节课数据

* 保存每节课数据 : SaveClass

>客户端请求格式:
 ```javascript
    data : {
       quizId: "xxx", //试题ID
       chat: [ //当前题目聊天内容 格式为数组 里面为多个聊天数据对象.
           {
               own: "xxx", // 发送人 类型
               msg: "xxx"  // 发送消息
           }
       ],
       boardUrl: "xxx" //上课画布存储URL
    }
 ```
 data: 存储数据

> 服务端处理:
  * 持久化储存

>```javascript
    result : {
      status: "xxx"
    }
 ```
 data: 存储信息

#####2.异步存储的同步切换保障

* 需要存储请求 : LocalAsyncSave

>客户端请求格式:
 ```javascript
    data : {}
 ```
 服务端处理:
 * 将数据原封不动转发给另一客户端

> ```javascript
     result : {}
  ```
 data: 数据为空

* 异步存储完毕 LocalAsyncSaveOK

>客户端请求格式:
 ```javascript
    data : {}
 ```
 服务端处理:
 * 将数据原封不动转发给另一客户端

> ```javascript
     result : {}
  ```
 data: 数据为空

#####3.获取服务器存储数据

* 获取服务器存储数据 : ServerSaveData

>```javascript
    data : {
      quizId: "xxx" //试题ID
    }
 ```
 data: 数据为空

> 服务端处理:
 * 返回此课程数据

>```javascript
    result : {
       quizId: "xxx", //试题ID
       chat: [ //当前题目聊天内容 格式为数组 里面为多个聊天数据对象.
           {
               own: "xxx", // 发送人 类型
               msg: "xxx"  // 发送消息
           }
       ],
       boardUrl: "xxx" //上课画布存储URL
    }
 ```
 data: 课程存储信息