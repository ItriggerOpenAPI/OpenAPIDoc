# 核销优惠券

### 接口描述

根据优惠券券码核销优惠券

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/coupons/consume?accessToken=ACCESSTOKEN&userCardCode=USERCARDCODE&userId=USERID66
```

### 请求方式

GET

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| userCardCode | String | 是 | 优惠券券码 |
| userId | Integer | 是 | 核销人Id\(确定门店\) |

### 返回数据示例

```text
{
    "code": 204,
    "message": "操作成功",
    "data": null
}
```

### 返回数据说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| code | int | 是 | 成功：200 失败：500 |
| message | String | 是 | 返回信息 |
| data | Obj | 否 | 目前没有数据返回,预留扩展 |



