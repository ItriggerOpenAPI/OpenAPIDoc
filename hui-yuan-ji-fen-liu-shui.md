---
description: '最后更新于：2019-06-12 18:44:06'
---

# 会员积分流水查询

### 接口描述

查询会员积分流水信息

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/member/point/list?accessToken=ACCESSTOKEN&mobile=MOBILE&pageNum=PAGENUM&pageSize=PAGESIZE
```

### 请求方式

GET

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| mobile | String | 是 | 手机号 |
| pageNum | int | 是 | 页码 |
| pageSize | int | 是 | 页面记录数 |

### 返回数据示例

```text
{
    "code":200,
    "message":"操作成功",
    "data":[
        {
            "id":473296,
            "exchangeTime":"2019-05-16 14:53:23",
            "detailReason":"营销活动",
            "exchangePoints":"100.0"
        }
    ],
    "total":1,
    "pageNum":1,
    "pageSize":10,
    "pageCount":1
}
```

### 返回数据说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| code | String | 是 | 成功：200，失败：500 |
| message | String | 是 | 返回详细说明 |
| data | String | 是 | 成功：true，失败：false |
| id | String |  | 记录id |
| exchangeTime | String |  | 修改时间 |
| detailReason | String |  | 修改原因 |
| exchangePoint | String |  | 修改积分 |
| total | int |  | 总记录数 |
| pageNum | int |  | 页码 |
| pageSize | int |  | 页面记录数 |
| pageCount | int |  | 总页数 |

