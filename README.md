# okteto部署vless

### 注册地址：https://okteto.com/

点击部署 |

![image](https://user-images.githubusercontent.com/89477009/133904828-38ef592c-ece3-45e7-a85e-812af23b756a.png)

按要求链接后，找到本项目 |

![image](https://user-images.githubusercontent.com/89477009/133905123-d40e3b72-49a5-46ca-9755-995f15dd49e5.png)  

部署就行了

 

### 变量

对部署时需设定的变量名称做如下说明：

UUID: 自行修改configure.sh文件中的UUID变量
路径：/app

# 通过 CloudFlare Workers 反向代理

```js
addEventListener(
    "fetch",event => {
    let url=new URL(event.request.url);
    url.hostname="xxx.cloud.okteto.net;
    let request=new Request(url,event.request);
    event. respondWith(
      fetch(request)
    )
  }
)
```

