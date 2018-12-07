# tool-charles

本篇为开发工具集中的第一篇。

charles，业界称为青花瓷，是 Mac 系统上最好用的一款用于 HTTP 请求的抓包工具。

## 下载

1、下载地址与破解说明：https://xclient.info/s/charles.html#versions

解压开有一个 keygen.jar，使用命令：java -jar keygen.jar 运行会出现注册所需信息。

2、官方下载：http://www.charlesproxy.com/download

## 使用教程

### 允许解析 http 请求

方法：

点击 顶部工具栏 Proxy-> Proxy settings ->proxies

勾选 enable transparent http proxying

效果图：

![](/images/http-setting.png)

### 允许解析 https 请求

方法：

点击 顶部工具栏 Proxy-> SSL Proxying Settings->SSL Proxying

勾选 Enable SSL Proxying

效果图：

![](/images/https-setting.png)

Configure your device to use Charles as its HTTP proxy on 192.168.66.234:8888, then browse to chls.pro/ssl to download and install the certificate.

Note that on iOS 10 and later you must then go into Settings > General > About > Certificate Trust Settings and enable the Charles certificate to be trusted.

### 真机抓包

1、查看电脑 IP

方法：

点击 系统偏好设置 -> 网络

![](/images/mac-ip.png)

2、设置 iPhone 网络

方法：

点击 设置 -> 无线局域网 -> 与电脑连接同一网络，点击右边的 i 进入配置，填写电脑的 IP 与端口，如：192.168.66.234:8888

![](/images/iphone-input-ip.png)

3、提示框

此处配置完成后，Charles 会弹出提示框，

大意是：有人请求连接 Charles ip 是 xxx.xxx.xxx.xxx 是否允许？
请选择 Allow

4、设置 iPhone SSL 证书

方法：

点击 设置 -> 通用 -> 关于本机 -> 证书，信任 charles 的证书

## 效果图

在手机浏览器，请求某个网站，如：www.liangyl.com ，请求抓取如下：

![](/images/charles-output.png)
