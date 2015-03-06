## WebRTC部分

##### 1.建立WebRTC点对点连接
* 创建Offer : RtcOffer

>客户端请求格式:
 ```javascript
    data : {
        sdp: "xxx"
    }
 ```
  服务端处理:
  * 将数据原封不动转发给另一客户端

>```javascript
    result : {
        sdp: "xxx"
    }
 ```
 data : sdp数据

* 创建Answer : RtcAnswer

>客户端请求格式:
 ```javascript
    data : {
        sdp: "xxx"
    }
 ```
  服务端处理:
  * 将数据原封不动转发给另一客户端

>```javascript
    result : {
        sdp: "xxx"
    }
 ```
 data : sdp数据

* 创建Ice : RtcIce

>客户端请求格式:
 ```javascript
    data : {
        ice: "xxx"
    }
 ```
  服务端处理:
  * 将数据原封不动转发给另一客户端

>```javascript
    result : {
        ice: "xxx"
    }
 ```
 data : ice数据

##### 3.关闭WebRTC

* 关闭WebRtc连接: RtcClose

>客户端请求格式:
 ```javascript
    data : {}
 ```
  服务端处理:
  * 将数据原封不动转发给另一客户端

>```javascript
    result : {}
 ```
 data : 空数据

##### 3.WebRTC异常处理

* WebRtc事件转发: RtcEvent

>客户端请求格式:
 ```javascript
    data : {}
 ```
  服务端处理:
  * 将数据原封不动转发给另一客户端

>```javascript
    result : {}
 ```
 data : 数据为任意