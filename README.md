基于[NoCortY](https://github.com/NoCortY)的项目[WebSSH](https://github.com/NoCortY/WebSSH)修改。
1. xterm版本升至4.X
2. terminal自适应宽高
3. 心跳检查
4. 断开后自动重新连接

**效果**

自适应宽高

![autoFit](https://raw.githubusercontent.com/mervynlam/Pictures/master/20200925100444.gif)

心跳检查

![heartbeat](https://raw.githubusercontent.com/mervynlam/Pictures/master/20200925101005.gif)

断开自动重连

![reconnect](https://raw.githubusercontent.com/mervynlam/Pictures/master/20200925101148.gif)


参考资料：  
[xterm.js + vue + websocket实现终端功能（xterm 3.x+xterm 4.x）](https://blog.csdn.net/weixin_38318244/article/details/103908129)  
[理解WebSocket心跳及重连机制（五）](https://www.cnblogs.com/tugenhua0707/p/8648044.html)

## 2020-3-13

最近有些事挺忙的，可能暂时稍微顺延一下更新的日程(大概需要在4月1号之后)，但是一定会继续维护下去的，望多多理解。

## 启动

项目导入IDEA后可以直接进行运行，没有任何外部依赖~~

**本项目的Blog**：[使用纯Java实现一个WebSSH项目](https://blog.objectspace.cn/2020/03/10/%E4%BD%BF%E7%94%A8%E7%BA%AFJava%E5%AE%9E%E7%8E%B0%E4%B8%80%E4%B8%AAWebSSH%E9%A1%B9%E7%9B%AE/)

**注意**：

由于前端代码中没有指定终端的信息

所以需要各位自己输入这些信息，位置在webssh.html中

```javascript
openTerminal( {
        /*operate:'connect',
        host: '',//IP
        port: '',//端口号
        username: '',//用户名
        password: ''//密码*/
    });
```

## 运行展示

- ### 连接

  ![连接](http://image.objectspace.cn/%E8%BF%9E%E6%8E%A5.png)

- ### 连接成功

  ![连接成功](http://image.objectspace.cn/%E8%BF%9E%E6%8E%A5%E6%88%90%E5%8A%9F.png)

- ### 命令操作

  ls命令：

  ![ls命令](http://image.objectspace.cn/ls%E5%91%BD%E4%BB%A4.png)

  vim编辑器:

  ![vim编辑器](http://image.objectspace.cn/vim%E7%BC%96%E8%BE%91%E5%99%A8.png)

  top命令：

  ![top命令](http://image.objectspace.cn/top%E5%91%BD%E4%BB%A4.png)
  
## 写在最后
欢迎各位大佬给我提issue，感谢！
