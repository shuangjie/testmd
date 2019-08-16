# 优越车网

## 产品分解

### 服务器搭建，分配四个站点

- wechat 

	- 微信公众号--客户端

- weapp

	-  微信小程序--客户端

- insurer

	- 子后台--保险公司端

- garage

	- 维修厂/美容店

- admin

	- 总后台管理系统

## 重点环节

### 发券系统，纳入监控系统，不能被无限发送

### 第三方api，如大润发卡，设定总量总阈值，控制出量

### 卡转系统，纳入监控系统，单一用户每天错误5次就要关闭该用户权限。

## 后台管理系统

### RBAC 权限管理

### 保司账户管理

- 额度
- 多管理员

### 发券系统

### 推送系统

### 报表统计

### 门店管理

### 影像系统

- 服务记录存档

## 保司-子后台

### RBAC 权限管理

### 员工账户管理

- 额度控制

### 发券系统

### 推送系统

### 报表统计

## 顾客-客户端

### 功能剖析

- 线上充值类服务

	- 手机话费
	- 手机流量
	- 腾讯视频、爱奇艺视频等视听会员
	- Q币等文娱充值
	- 通用礼品卡
	- 加油卡充值
	- 加油卡代充

- 线下服务

	- 标准洗车
	- 精致洗车
	- 标准打蜡
	- 抛光打蜡
	- 机油套餐
	- 喷漆套餐

- 增值服务

	- 年审代办
	- 违章查询
	- 24项安全检查
	- 道路救援

- 个人中心

	- 我的资料
	- 我的订单
	- 我的卡券
	- 我的钱包

- 在线客服
- 反馈与建议

### 前端

- 首页
- 线上服务

	- 手机充值页面
	- 视听会员充值页面
	- 礼品卡页面
	- QQ会员/Q币充值页面
	- 油卡充值页面
	- 支付页面
	- 绑定加油卡页面

- 线下服务

	- 洗车/打蜡等商品页
	- 服务网点页面

- 个人中心

	- 个人中心主页
	- 余额充值
	- 卡券领取
	- 我的订单
	- 我的资料
	- 反馈与建议
	- 我的消息

- 我的卡券

	- 已使用
	- 未使用
	- 已过期

### 后端

- 第三方充值api
- 用户基本信息

	- curd

- 商品
- 支付
- 订单
- 我的账户
- 我的卡券
- 反馈与建议
- 通知

### 数据库

- 用户表
- 广告表
- 第三方api列表
- 充值记录
- 账户流水表
- 卡券领取表
- 卡券兑换表
- 卡券表
- 卡券使用表
- 订单表
- 用户账户表
- 反馈与建议表
- 消息表

## 维修厂/美容店端

### 功能剖析

- 预约列表
- 我的订单
- 我的钱包

	- 结算(走线下流程，线上标记)

- 扫码核销

### 前端

- 首页

	- 扫码核销

		- 存档（影像）

- 预约列表
- 个人中心

	- 我的订单
	- 我的钱包

		- 结算

	- 反馈与建议
	- 客服

### 后端

- 扫码核销
- 核销上传/资料存档
- 我的订单
- 预约列表
- 客服消息转发到微信
- 反馈与建议
- 我的钱包相关

### 数据库

- 商家表
- 用户表
- 预约记录表
- 服务使用表
- 扫码核销记录
- 核销存档影像
- 反馈与建议

## 卡转-回收平台

### 客户端

- 功能剖析

	- 卡券回收
	- 个人中心
	- 转让记录
	- 推送
	- 客服

- 前端

	- 首页
	- 卡券转让
	- 转让记录
	- 个人中心

		- 绑定手机号码
		- 账户余额
		- 提现
		- 提现设置

			- 支付宝
			- 微信
			- 银联

	- 客服（结合微信客服系统）

### 后台

- 监控系统

	- 按分/时/天三个规则进行限制
	- 通知系统

		- 分发警报信息到管理员

- 报表统计
- 回收管理
