---
description: '最后更新于：2019-09-20 15:44:06'
---

# 订单创建/更新

### 接口描述

完成订单的新建和更新操作

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/order/platform/trades?accessToken=ACCESSTOKEN
```

### 请求方式

POST

### 请求数据示例

```text
{
	"buyerNick": "测试",
	"originalContent":"",
	"platformCode": "taobao",
	"platformTradeCode": "49913134",
	"sellerNick": "达子",
	"shopName": "企加云店铺"
	"createTime": "2019-05-10 16:55:49"
}
```

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| platformCode | String | 是 | 平台code |
| platformTradeCode | String | 是 | 平台订单编码 |
| shopName | String | 是 | 店铺名称 |
| originalContent | String | 是 | platformCode对应平台的订单格式，比如天猫平台订单内容为：{"address":"杭州滨江聚光B-17","brandId":1,"buyerMemo":"","buyerNick":"","consignee":"李强","mobile":"13720534766","orderList":\[{"brandId":1,"goodsCount":1,"payment":"999999","platformOrderCode":"1234567890","platformProductCode":"123123","productCode":"123123","productName":"鲜花","productSkuCode":"1231234","productSkuName":"白色鲜花","status":10,"tenantId":12818}\],"orderTime":"","payTime":"2019-08-13 00:50:50","payment":"99999","platformCode":"pos","platformTradeCode":"123456789","shopName":"","status":10,"storeId":1,"storeName":"测试门店","tenantId":12818,"totalAmount":"99999","type":1} |
| buyerNick | String | 否 | 买家昵称 |
| sellerNick | String | 否 | 卖家昵称 |
| createTime | String | 否 | 订单创建时间 |

### 返回数据示例

```text
{
  "code": 200,
  "data": true,
  "message": "操作成功"
}
```

### 返回数据说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| code | String | 是 | 成功：200，失败：500 |
| message | String | 是 | 返回详细说明 |
| data | String | 是 | 成功：true，失败：false |

