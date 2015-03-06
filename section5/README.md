## 功能性按钮部分

#####1.切换上课题目

* 切换上课题目 : SwitchTopics (此功能需要根据后端数据处理进行讨论)

>客户端请求格式:
 ```javascript
    data : {
        classId: "xxx"
    }
 ```
  服务端处理:
  * 将数据原封不动转发给另一客户端

>```javascript
    data : {
        classId: "xxx"
    }
 ```
 data: 上课题目所对应的id