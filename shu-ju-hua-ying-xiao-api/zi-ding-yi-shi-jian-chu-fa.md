---
description: '最后更新于：2019-09-27 15:44:06'
---

# 自定义事件触发

### 接口描述

第三方可以调用此接口触发在系统中已配置的自定义事件

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/event/trigger?accessToken=ACCESSTOKEN
```

### 请求方式

POST

### 请求数据示例

```text
{
	"personId": "123",
	"brandId": "12",
	"eventCode": “custom_code_1",
	"eventTime": "2018-07-20 12:12:12",

	“custom_condition_1”:”123”,
	“custom_condition_2”:”123”
	...
}
```

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| personId | String | 是 | 事件发生人ID |
| brandId | String | 是 | 所属品牌 |
| eventCode | Integer | 是 | 事件编码 |
| eventTime | String | 否 | 事件发生时间 |
| 其他参数 |  | 否 | campaign-data schema 中event\_attribute表配置的其他事件属性，详见自定义事件使用文档 |

### 返回数据示例

```text
{
  "code": 200,
  "message": "操作成功"
}
```

### 返回数据说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| code | String | 是 | 成功：200，失败：500 |
| message | String | 是 | 返回详细说明 |

