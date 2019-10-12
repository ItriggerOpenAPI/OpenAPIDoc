---
description: '最后更新于：2019-09-20 15:44:06'
---

# 订单退单

### 接口描述

完成订单的退单操作

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/order/platform/refunds?accessToken=ACCESSTOKEN
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
| id | Long | 是 | id |
| platformCode | String | 是 | 平台code |
| platformRefundCode | String | 是 | 原始退款单号 |
| shopName | String | 是 | 店铺名称 |
| refundContent | String | 是 | platformCode对应平台的退单格式，比如天猫平台订单内容为：{ "refund\_get\_response": { "refund": { "refund\_id": "16039173514059992", "status": "SUCCESS", "seller\_nick": "企加云123", "buyer\_nick": "~6PL+lwkmXmLKiBVT+GVmDw==~1~", "tid": 226529926389059299, "oid": 226529926389059299, "created": "2019-04-28 17:32:53", "modified": "2019-04-28 17:32:54", "advance\_status": 0, "alipay\_no": "2018101322001109190515915461", "attribute": "", "cs\_status": 1, "desc": "", "good\_status": "BUYER\_NOT\_RECEIVED", "has\_good\_return": false, "num": 1, "num\_iid": 576119468732, "operation\_contraint": "null", "order\_status": "TRADE\_CLOSED", "payment": "0.00", "price": "0.10", "reason": "拍错/多拍/不想要", "refund\_fee": "0.10", "refund\_phase": "onsale", "refund\_version": 1556443973380, "sku": "3791806308316\|颜色分类:黑色\[黑色\]", "title": "毛线", "total\_fee": "0.10" } } } |
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

