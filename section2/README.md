## 画板部分

##### 1.画布数据传输
* 画画布 : BoardDraw

>客户端请求格式:
 ```javascript
  data : {
      draw: [
          n*[
              n*{}
          ]
      ]
  }
 ```
 服务端处理:
 * 将数据原封不动转发给另一客户端

>```javascript
  result : {
      draw: [
          n*[
              n*{}
          ]
      ]
  }
  ```
  data : 数据为一个二维数据 里面有多个 obj (画笔在动画每秒60次循环中, 每次取到的路径点, 与绘图状态)<br/>

##### 2.画布功能性操作
* 切换到橡皮模式 : BoardControl

>客户端请求格式:
 ```javascript
    data : {
        type: 'eraser'
        data: {} //可有可无
    }
 ```
 服务端处理:
 * 将数据原封不动转发给另一客户端

>```javascript
   result : {
        type: 'eraser'
        data: {} //可有可无
   }
 ```
 data : 数据为操作方法名字