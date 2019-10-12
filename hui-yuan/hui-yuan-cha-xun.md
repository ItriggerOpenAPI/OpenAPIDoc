---
description: '最后更新于：2019-06-12 18:44:06'
---

# 会员查询

### 接口描述

查询会员信息

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/member/query?accessToken=ACCESSTOKEN&mobile=MOBILE&storeNo=STORENO
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
	"code": 200,
    "message": "操作成功",
    "data": {
        "realName": "杜代亮",
        "gender": "male",
        "birthDay": "1993-09-12 00:00:00",
        "identity": "23444444123",
        "county": "昌平区",
        "province": "北京市",
        "city": "北京",
        "address": "云广场D座南门",
        "headPic": "www.baidu.com",
        "growth": "100",
        "levelName": "一级",
        "point": "1100.0"
    }
}
```

### 返回数据说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| code | String | 是 | 成功：200，失败：500 |
| message | String | 是 | 返回详细说明 |
| data | Object | 否 | 会员具体信息对象 |
| realName | String |  | 姓名 |
| gender | String |  | 性别 |
| birthDay | String |  | 生日 |
| identity | String |  | 身份证 |
| county | String |  | 郡县 |
| province | String |  | 省份 |
| city | String |  | 城市 |
| address | String |  | 地址 |
| headPic | String |  | 头像 |
| growth | String |  | 成长值 |
| levelName | String |  | 等级名称 |
| point | String |  | 积分 |



