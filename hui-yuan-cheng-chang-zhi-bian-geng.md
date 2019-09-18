---
description: '最后更新于：2019-06-12 18:44:06'
---

# 会员成长值变更

### 接口描述

主动调用该接口，更改会员成长值，等级有可能随着成长值的变化而变化

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/member/growth/modify?accessToken=ACCESSTOKEN
```

### 请求方式

POST

### 请求数据示例

```text
{
  "changeDesc": "后台手动增加",
  "changeGrowth": 10,
  "changeTime": "2019-09-09 12:23",
  "effectiveTime": "2019-09-15",
  "invalidTime": "2019-09-25",
  "mobile": "18880009999",
  "operation": "add",
  "reasonText": "后台手动修改",
  "reasonType": 3
}
```

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| mobile | String | 是 | 手机号 |
| changeDesc | String | 是 | 变更原因 |
| changeGrowth | String | 否 | 变更成长值数量 |
| changeTime | String | 否 | 变更时间：2019-01-02 |
| effectiveTime | String | 否 | 生效时间 |
| invalidTime | String | 否 | 失效时间 |
| operation | String | 否 | 操作add:加,sub:减 |
| reasonText | String | 否 | 变更类型文本 |
| reasonType | String | 否 | 变更类型id |

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

