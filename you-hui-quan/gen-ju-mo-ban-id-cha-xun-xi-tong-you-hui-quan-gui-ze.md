---
description: '最后更新于：2019-07-12 15:44:06'
---

# 根据模板查询系统优惠券规则

### 接口描述

使用优惠券模板id查询系统优惠券规则

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/coupons/detail/byTemplateId?accessToken=ACCESSTOKEN&templateId=TEMPLATEID
```

### 请求方式

GET

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| templateId | String | 是 | 优惠券模板id |

### 返回数据示例

```text
{
    "code": 200,
    "message": "操作成功",
    "data": {
        "id": 110,
        "title": "球的系统折扣券",
        "couponType": "DISCOUNT",
        "getLimit": 5,
        "quantity": "100",
        "is_superimposed": false,
        "canGiveFriend": false,
        "useCondition": null,
        "beginTimestamp": 1556647800000,
        "endTimestamp": 1562903400000,
        "description": "3.3",
        "properStore": "96,113,97,98,99,85,94",
        "useAllLocations": false,
        "defaultDetail": null,
        "couponReceiveRecordId": 2486,
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



