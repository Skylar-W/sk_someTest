# WebSocket原理

# 聊天室
  - 前端
  1. Login
     用户名输入/进入聊天室的按钮
     input username(至少6位) --> localStorage --> enter chatting room

  2. Home
     消息列表/消息输入框/发送按钮
     localStorage --> username/msg/id/time --> 后端socket服务

    + 事件驱动
      - open
      - close
      - error
      - message   接收广播来的数据

  - 后端
     接收 --> 消息数据 --> 广播给所有连接到socket服务的客户端

    + 事件驱动
      - open
      - close
      - error
      - connection
        + message   接收客户端发送的消息数据 --> 广播出去







> websocket2

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
