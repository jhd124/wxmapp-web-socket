# wxmapp-web-socket
# 小程序websocket接头
## 为什么？
有时候我们开发了一个websocket应用，想把它移植到微信小程序上，或是想使用依赖于websocket的库，然而小程序API提供的socket接口不是标准的websocket接口，无法在上述场景内直接应用。这个库以小程序socket API为基础实现了websocket的接口。
## 安装
```
npm install --save wxmapp-web-socket 
```
或 
```
yarn add wxmapp-web-socket
```
## 使用
```
import { WrappedWxSocket } from "wxmapp-web-socket";

const url = "wss://somewhere.com"
const websocket = new WrappedWxSocket(url)

```