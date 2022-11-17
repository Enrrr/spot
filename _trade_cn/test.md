---
title: 完整ticker
position_number: 7
## 获取交易对的最新成交信息


**接口地址**:`/v1/q/deal`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|num|数量|query|true|integer(int64)||
|symbol|交易对|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|CommonResponse«List«DealVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code||integer(int32)|integer(int32)|
|data||array|DealVO|
|&emsp;&emsp;a|成交量|number(bigdecimal)||
|&emsp;&emsp;m|买卖方向|string||
|&emsp;&emsp;p|成交价|number(bigdecimal)||
|&emsp;&emsp;s|交易对|string||
|&emsp;&emsp;t|成交时间|integer(int64)||
|msg||string||


**响应示例**:
```javascript
{
    "code": 0,
    "data": [
        {
            "a": 0,
            "m": "",
            "p": 0,
            "s": "",
            "t": 0
        }
    ],
    "msg": ""
}
```
---
