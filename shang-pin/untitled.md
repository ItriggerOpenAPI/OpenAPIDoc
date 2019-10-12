---
description: '最后更新于：2019-09-20 15:44:06'
---

# 商品创建/更新

### 接口描述

完成商品的新建和更新操作

### 接口地址

```text
https://gateway-dev.itrigger.cn/itrigger-bff/v2/open/api/product/sys/products?accessToken=ACCESSTOKEN
```

### 请求方式

POST

### 请求数据示例

```text
{
  "barcode": "TEST11233",
  "descModules": "xxxx",
  "goodsCostPrice": "12.88",
  "goodsManufactureDate": "2018-07-20 12:12:12",
  "goodsManufacturer": "浙江杭州xxx商品厂",
  "goodsOrigin": "浙江杭州",
  "goodsPrice": "20.88",
  "goodsWeight": "50",
  "itemImgs": "xxxx.png",
  "memo": "xxx",
  "name": "辣条",
  "code": "AEF123234",
  "type": 1,
  "picUrl": "xxxx1.png",
  "supplierName": "xxxx",s
  "unit": "克"
}
```

### 请求参数说明

| 参数名称 | 参数类型 | 是否必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| name | String | 是 | 商品名称 |
| code | String | 是 | 商品编号 |
| type | Integer | 是 | 商品类型（虚拟/实物/服务等） |
| barcode | String | 否 | 商品条码 |
| brandId | Integer | 否 | 商品品牌 |
| goodsCostPrice | String | 否 | 商品成本价 |
| goodsManufactureDate | String | 否 | 生产日期 |
| goodsManufacturer | String | 否 | 生产厂商 |
| goodsOrigin | String | 否 | 商品产地 |
| goodsPrice | String | 否 | 商品售价 |
| goodsWeight | String | 否 | 商品重量 |
| itemImgs | String | 否 | 商品多图地址 |
| memo | String | 否 | 备注 |
| picUrl | String | 否 | 商品主图地址 |
| supplierId | Integer | 否 | 供应商ID |
| supplierName | String | 否 | 供应商名称 |
| unit | String | 否 | 单位 |
| descModules | String | 否 | 商品详细描述 |

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

