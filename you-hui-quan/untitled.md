---
description: '最后更新于：2019-07-12 15:44:06'
---

# 根据券码查询系统优惠券规则

### 接口描述

使用优惠券券码查询系统优惠券规则

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/coupons/detail/byUserCardCode?accessToken=ACCESSTOKEN&userCardCode=USERCARDCODE
```

### 请求方式

GET

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| userCardCode | String | 是 | 优惠券券码 |

### 返回数据示例

```text
{
    "code": 200,
    "message": "操作成功",
    "data": {
        "id": 102,
        "title": "系统导购券",
        "couponType": "GENERAL_COUPON",
        "getLimit": 10,
        "quantity": "1000",
        "is_superimposed": false,
        "canGiveFriend": false,
        "useCondition": null,
        "beginTimestamp": 1557904304000,
        "endTimestamp": 1566544304000,
        "description": "1",
        "properStore": null,
        "useAllLocations": true,
        "defaultDetail": "1",
        "couponReceiveRecordId": 2365,
        "remark": null
    }
}
```

### 返回数据说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| beginTimestamp | String |  | 优惠券使用期限\(开始时间\) |
| canGiveFriend | boolean |  | 是否支持转赠 |
| couponReceiveRecordId | integer |  | 接收的优惠券id |
| couponType | String |  | 优惠券类型 |
| defaultDetail | String |  | 优惠券说明 |
| description | String |  | 代金券代表金额折扣券代表折扣等 |
| endTimestamp | String |  | 优惠券使用期限\(结束时间\) |
| getLimit | String |  | 每人限领数 |
| id | integer |  | 优惠券模板id |
| is\_superimposed | boolean |  | 是否可叠加 |
| properStore | String |  | 适用门店\(微信支付无\) |
| quantity | String |  | 总发行量 |
| remark | String |  | 优惠券备注 |
| title | String |  | 优惠券名称 |
| useAllLocations | boolean |  | 是否所有门店适用 |
| useCondition | String |  | 使用门槛 |



