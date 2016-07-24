# [Yinle][1] API for Web & Android

> **印乐**：一键式自助打印服务，截止目前(2016-07-23)为大连多所高校提供自助打印服务。

## 关于
- 本项目是对**印乐**提供的Web和Android客户端的接口分析，**非官方**



## Android

- 替换 **手机号** 13800138000
- 替换 **user_id** 911
- 替换 **fileid** 20550
- yinle.cc == 121.42.15.77

### 获取支持地点列表
http://yinle.cc/Ajax//AjaxUser.aspx?oper=getalladdress

### 获取专业分类列表
http://yinle.cc/Ajax//AjaxUser.aspx?oper=getallmajor

### 获取安卓最新版本号
http://yinle.cc/Ajax/ajaxadmin.aspx?oper=getandroidvid

### 最新活动列表
http://wx.yinle.cc/activity/getactivity.json

### 获取user_id 昵称和头像由手机号
http://yinle.cc/Ajax//AjaxUser.aspx?oper=havephonesj&phone=13800138000

### 登录 获取token和帐号状态等
http://yinle.cc/Ajax//AjaxUser.aspx?oper=login&phone=13800138000&pwd=123456

### 获取用户信息由user_id
http://yinle.cc/Ajax//AjaxUser.aspx?oper=getuserinfo&userid=911

### 签到
http://yinle.cc/Ajax//AjaxUser.aspx?oper=usersign&userid=911

### 订单 待付款
http://yinle.cc/Ajax/AjaxOrder.aspx?oper=getorderinfo&status=3&userid=911

### 订单 待打印
http://yinle.cc/Ajax//AjaxOrder.aspx?oper=getnoprint&userid=911

### 订单 已打印
http://wx.yinle.cc/pc/getorderinfobyuseridandstatus.json?callback=jsonp&userid=911&status=1&pagecount=0&pagesize=1000

### 获取用户已上传文件的列表
http://yinle.cc/Ajax//AjaxFile.aspx?oper=getmyfilebyname&userid=911&filename=

### 删除文件
- fileid非userid所有 亦可
http://yinle.cc/Ajax//AjaxFile.aspx?oper=deletefilebyfileid&fileid=20550&userid=911

### 打印文件
http://yinle.cc/Ajax//AjaxOrder.aspx?oper=pinrtfile&fileid=20550&userid=911

### 删除待打印订单
http://yinle.cc/Ajax//AjaxOrder.aspx?oper=deleteorderbyorderid&userid=911&orderid=1469292050456962



[1]:http://www.yinle.cc/
