<p>
<img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=86400" />
  <a href="#" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-green.svg" />
  </a>
  <a href="https://twitter.com/xiaomoinfo" target="_blank">
    <img alt="Twitter: xiaomoinfo" src="https://img.shields.io/twitter/follow/xiaomoinfo.svg?style=social" />
  </a>
</p>

# 准备运行环境
```
go mod tidy 
cp config/config.yaml.example local/config.yaml
```

## 修改你的token
打开 [openai](https://beta.openai.com/account/api-keys) 并注册一个账号, 生成一个token并把token放到

## 运行App
```
go run main.go
```

```
ain.go #gosetup
go: downloading github.com/eatmoreapple/openwechat v1.2.1
go: downloading github.com/sirupsen/logrus v1.6.0
go: downloading github.com/spf13/afero v1.9.2
go: downloading github.com/pelletier/go-toml/v2 v2.0.5
go: downloading golang.org/x/sys v0.0.0-20220908164124-27713097b956
/private/var/folders/8t/0nvj_2kn4dl517vhbc4rmb9h0000gn/T/GoLand/___go_build_main_go
访问下面网址扫描二维码登录
https://login.weixin.qq.com/qrcode/QedkOe1I4w==
```

会自动打开默认浏览器，如果没有打开也可以打动点击上面的链接打开二维码扫微信

```
2022/12/09 15:15:00 登录成功
2022/12/09 15:15:01 RetCode:0  Selector:2
2022/12/09 15:15:04 RetCode:0  Selector:2
INFO[0099] 0 <Friend:hxh,晓华>                            
INFO[0099] 1 <Friend:刘葵>                                
INFO[0099] 2 <Friend:吕>                                 
INFO[0099] 3 <Friend:wloscar>               
```
登陆成功后会拉取微信的好友和群组

## 如何使用
默认为`chatgpt`，如果想设置其他的触发方式可以修改`local/config.yaml`的keyword。此时，如果别人给你发消息带有关键字`chatgpt`，你的微信就会调整用`chaget`AI自动回复你的好友。


