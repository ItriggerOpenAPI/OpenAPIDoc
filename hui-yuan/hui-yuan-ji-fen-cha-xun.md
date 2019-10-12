---
description: '最后更新于：2019-06-12 18:44:06'
---

# 会员积分查询

### 接口描述

查询会员剩余积分

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/member/point?accessToken=ACCESSTOKEN&mobile=MOBILE&storeNo=STORENO
```

### 请求方式

GET

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| mobile | String | 是 | 手机号 |
| storeNo | String | 是 | 门店编号 |

### 返回数据示例

```text
{
    "code":200,
    "message":"操作成功",
    "data":{
        "currentPoint":100
    }
}
```

### 返回数据说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| code | String | 是 | 成功：200，失败：500 |
| message | String | 是 | 返回详细说明 |
| data | String | 是 | 成功：true，失败：false |
| currentPoint | Double | 是 | 会员剩余积分 |

