---
description: '最后更新于：2019-06-12 18:44:06'
---

# 会员修改

### 接口描述

修改会员信息，需要修改哪些字段，就传哪些字段

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/member/modify?accessToken=ACCESSTOKEN
```

### 请求方式

POST

### 请求数据示例

```text
{
  "address": "云广场D座南门",
  "birthDay": "1993-09-12",
  "city": "北京",
  "county": "海淀区",
  "gender": "male",
  "mobile": "18899888899",
  "province": "北京市",
  "realName": "杜代亮"
}
```

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| mobile | String | 是 | 手机号 |
| address | String | 否 | 详细地址 |
| birthDay | String | 否 | 生日：2019-01-02 |
| city | String | 否 | 城市 |
| county | String | 否 | 郡县 |
| gender | String | 否 | 性别 male female |
| headPic | String | 否 | 头像地址 |
| identity | String | 否 | 身份证 |
| province | String | 否 | 省份 |
| realName | String | 否 | 姓名 |

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

