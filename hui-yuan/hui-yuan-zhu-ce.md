# 会员注册

### 接口描述

注册会员，通过此接口完成多渠道的会员注册功能

### 接口地址

```text
https://gateway-mb-dev.itrigger.cn/itrigger-bff/v2/open/api/member/register?accessToken=ACCESSTOKEN
```

### 请求方式

POST

### 请求数据示例

```text
{
  "mobile": "18899888899",
  "storeNo": "1159374785466208256"
  "address": "西二旗软件园云广场",
  "birthday": "2019-07-30",
  "brandId": 1,
  "channel": "16",
  "city": "北京",
  "county": "昌平区",
  "gender": "male",
  "headpic": "www.baidu.com",
  "identity": "23444444123",
  "province": "北京",
  "realName": "小伙伴"
}
```

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| mobile | String | 是 | 手机号 |
| storeNo | String | 是 | 门店编号 |
| channel | String | 是 | 注册渠道 |
| address | String | 否 | 详细地址 |
| birthDay | String | 否 | 生日：2019-01-02 |
| channelId | String | 否 | 渠道标识 |
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

