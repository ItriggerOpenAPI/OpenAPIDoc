---
description: '最后更新于：2019-07-12 15:44:06'
---

# 优惠券券码发送



### 接口描述

根据会员渠道信息或手机号发送相应优惠券模板id的优惠券; 手机号或渠道信息二者必传一个

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/coupons/divide?accessToken=ACCESSTOKEN
```

### 请求方式

POST

### 请求数据示例

```text
{
  "channelRecoginizeId": 66,
  "channelType": "WX",
  "couponId": 20,
  "phones": [
    "18612323698"
  ],
}
```

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| channelRecoginizeId | integer | 否 | 渠道身份识别id |
| channelType | integer | 否 | 渠道类型 |
| couponId | integer | 是 | 优惠券模板ID |
| phone | String | 否 | 电话号码 |

### 返回数据示例

```text
{
    "code": 200,
    "message": "操作成功",
    "data": [
        2497
    ]
}
```

### 返回数据说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| code | String | 是 | 成功：200，失败：500 |
| message | String | 是 | 返回详细说明 |
| data | String | 是 | 发送成功的优惠券id列表 |

