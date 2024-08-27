```terminal
oktica@dev$ post_recommend.md
```

<div align="center">
  <a href="https://setbun.com/">
    <img src="logo-final/oktica-right-logo-neon-webkit-animation.svg" width="300px"/>
    <br>
    <img src="https://profile-counter.glitch.me/FrederickAsYou/count.svg"/>
  </a>
</div>


> [!CAUTION]
> For testimonials only, please check out the [blog](https://www.setbun.com) for more information

## Pixel-Chat是啥？

哎，最近在集训，本来说发了项目就更博，结果拖到<kbd>Boom</kbd>项目还没发

这是我最近和朋友写的一个[即时聊天](https://www.bing.com/search?q=%E5%8D%B3%E6%97%B6%E8%81%8A%E5%A4%A9&PC=U316&FORM=CHROMN)项目，项目地址：[https://github.com/AlignPixel/Pixel-Chat-App](https://github.com/AlignPixel/Pixel-Chat-App)

欢迎点Star支持

具体说明请阅读项目的 `README.md`，这里就不过多赘述

## 那Pixel-Chat Boom又是啥？

~~好的，我来说说~~

他是一个用于测试服务端性能的玩意，原理是通过不断访问来挑出BUG

#### 有BUG咋整？

~~好问题~~

如果您自己能够解决，那么你可以自行更改服务端，若你想帮助大家还可以为项目提交PR，大家共同进步

如果您自己不能够解决，那么请你提一个issue，等待大家帮你解决

### 废话这么多，那我问你：“咋用啊？”

本项目本身就是循环访问，所以是直接修改客户端文件，这里给出样本

```pixel-chat-boom.py
import json
import threading
from socket import *

is_login = False
is_broadcast = True

# 接受消息类，一般不要更改，容易和服务端出现数据不对号等错误
class ClientReceiveThread(threading.Thread):
    __buf = 1024
    # 初始化
    def __init__(self, cs):
        super(ClientReceiveThread, self).__init__()
        self.__cs = cs

    def run(self):
        self.receive_msg()



## ... please go to the blog for more information
```

大概就是这个样子，官方不提供此技术支持，如果你有问题请到[项目讨论](https://github.com/AlignPixel/Pixel-Chat-App/discussions)与其他小伙伴交流、分享测试经验

## 声明

本项目仅供测试程序，禁止用作违法违规用途，发生事故本人概不负责！

---

###### &copy; 2024 Frederick Chen. All rights reserved. 
