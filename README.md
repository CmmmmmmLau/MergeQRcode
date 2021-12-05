# MergeQRcode
将微信和支付宝的收款码二合一.支持自定义二维码样式,但是没有面板的DIY.

## MergeQRcode V1(废案)
该方案为废案,因为二维码的生成实现在了HTML的画布(Cansav)上.
而微信内置浏览器的二维码扫描只能识别`<img>`标签的图片.
虽然该库提供了方法获取源数据,但是返回的值是`Blob`类型而我没有系统学习过JS.
因此作废.
### 使用方法
1.下载源码并部署到自己的网站上

2.获取自己的二维码,通过第三方网站识别获取二维码的内容.

3.将识别出来的链接替换掉源码中的链接即可.

[Demo](https://cmmmmmm.com/qrcode/MergeQRcode.html)

## MergeQRcode V2
相比V1,V2使用的生成库的自定义程度更高.
虽然二维码的生成也是基于画布实现的,但是因为可以导出Base64图片.
不过对二维码的样式更新并没有像上一个方法一样便捷直接提供了`update()`方法.需要清除二维码,更改参数并重生生成二维码.

### 使用方法
1.`npm install easyqrcodejs`

2.剩余步骤同上个方案

[Demo](https://cmmmmmm.com/qrcode/MergeQRcode2.html "Demo")
