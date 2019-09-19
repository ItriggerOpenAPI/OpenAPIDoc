# 查询优惠券列表

### 接口描述

外部系统根据会员渠道信息或手机号查询会员优惠券列表,手机号或渠道信息二者必传一个

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/coupons/list?accessToken=ACCESSTOKEN
```

### 请求方式

POST

### 请求数据示例

```text
{
  "channelRecoginizeId": 0,
  "channelType": 0,
  "pageNum": 0,
  "pageSize": 0,
  "phone": "string",
  "tenantId": 0
}
```

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| channelRecoginizeId | integer | 否 | 渠道身份识别id |
| channelType | integer | 否 | 渠道类型 |
| pageNum | integer | 是 | 页码数 |
| pageSize | integer | 是 | 页内数量 |
| phone | String | 否 | 电话号码 |

### 返回数据示例

```text
{
    "code": 200,
    "message": "操作成功",
    "data": [
        {
            "id": 111,
            "userCardCode": "201905161627142210201FTt3hm12818",
            "status": "未使用"
        }
    ],
    "total": 0,
    "pageNum": 0,
    "pageSize": 0,
    "pageCount": 0
}
```

### 返回数据说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| code | String | 是 | 成功：200，失败：500 |
| message | String | 是 | 返回详细说明 |
| data | String | 是 | 成功：true，失败：false |
| id | integer |  | 优惠券模板id |
| userCardCode | String |  | 优惠券券码 |
| status | String |  | 优惠券状态\(已使用、未使用、已过期\) |
| pageCount | integer |  | 总页数 |
| pageNum | integer |  | 当前页 |
| pageSize | integer |  | 每页条数 |
| total | integer |  | 总条数 |

