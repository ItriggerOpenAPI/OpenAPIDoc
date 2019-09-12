---
description: '最后更新于：2019-06-12 18:44:06'
---

# 会员绑定

### 接口描述

指定渠道的会员绑定

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/member/binding?accessToken=ACCESSTOKEN
```

### 请求方式

POST

### 请求数据示例

```text
{
  "mobile": "18899888899",
  "channel": "2",
  "channelId": "这里填有效的微信openId"
}
```

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| mobile | String | 是 | 手机号 |
| channel | String | 是 | 渠道类型 |
| channelId | String | 是 | 渠道标示 |

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

