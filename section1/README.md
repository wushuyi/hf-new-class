## 数据传输规范

##### 1.WebSocket 传输数据格式规定
* 采用socket.io 作为传输层

* socket.io 原生事件名字为 onData

* 事件格式规范:
>1. 客户端请求浏览器前缀为 req => 'request'
 2. 服务端返回前缀为 res => 'response'
 3. 事件命名规则采用驼峰命名法

* 数据格式为:
> 服务端数据格式:
 ```json
    {
     "success": "[true||false]",
     "info": "[string]",
     "type": "[string]",
     "code": "[string]",
     "result": "[json]"
    }
 ```
 success : 服务端是否操作成功<br/>
 info : 服务端返回的信息<br/>
 type : 指定ws调用的命名空间<br/>
 code : 调用的接口名字<br/>
 result : 服务端返回的数据<br/>
 ******
 客户端数据格式:
 ```json
    {
     "type": "[string]",
     "code": "[string]",
     "data": "[json]"
    }
 ```
 type : 指定ws调用的命名空间<br/>
 code : 调用的接口名字<br/>
 data : 服务端返回的数据<br/>