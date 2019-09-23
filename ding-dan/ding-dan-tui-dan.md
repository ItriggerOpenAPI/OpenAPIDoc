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
| refundContent | String | 是 | 原始订单数据json |
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

