## 获取上课题目部分

#####1.获取上课题目列表

* 获取上课题目列表 : ClassList

>客户端请求格式:
 ```javascript
    data : {}
 ```
 data: 数据为空

> 服务端处理:
  * 发送上课列表到请求端

>```javascript
    result : {
        classList: [], //此数据格式有待讨论, 前端希望是排列好的数组
        currQuizId: "xxx" //可有可无 , 如果上一次为异常退出则发送 上次异常课程ID
    }
 ```
 data: 上课列表数据