# oktetov2

### 注册地址：https://okteto.com/

点击部署 ![image](https://user-images.githubusercontent.com/89477009/133904828-38ef592c-ece3-45e7-a85e-812af23b756a.png)
按要求链接后，找到本项目 ![image](https://user-images.githubusercontent.com/89477009/133905123-d40e3b72-49a5-46ca-9755-995f15dd49e5.png)  部署就行了

 

### 变量

对部署时需设定的变量名称做如下说明。

| 变量 | 默认值 | 说明 |
| :--- | :--- | :--- |
| `ID` | `ad806487-2d26-4636-98b6-ab85cc8521f7` | VMess 用户主 ID，用于身份验证，为 UUID 格式 |
| `AID` | `64` | 为进一步防止被探测所设额外 ID，即 AlterID，范围为 0 至 65535 |
| `WSPATH` | `/` | WebSocket 所使用的 HTTP 协议路径 |

## 接入 CloudFlare

以下两种方式均可以将应用接入 CloudFlare，从而在一定程度上提升速度。

 1. 为应用绑定域名，并将该域名接入 CloudFlare
 2. 通过 CloudFlare Workers 反向代理


