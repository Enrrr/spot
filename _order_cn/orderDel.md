---
title: 撤销订单
position_number: 3
type: post
split: '-------------------------------------'
description: |
    接口地址:/v1/order/cancel  <br>请求数据类型:application/x-www-form-urlencoded
parameters:
    -
        name: orderId
        type: number
        mandatory: false
        default:
        description: 订单ID
        ranges:
content_markdown: |-
    **请求参数**\:

    | 参数名称 | 参数说明 | 请求类型 | 是否必须 | 数据类型 | schema |
    | --- | --- | --- | --- | --- | --- |
    | orderId | 订单Id | query | true | integer(int64) | &nbsp; |

    **响应状态**\:

    | 状态码 | 说明 | schema |
    | --- | --- | --- |
    | 200 | OK | CommonResponse&laquo;object&raquo; |
    | 201 | Created | &nbsp; |
    | 401 | Unauthorized | &nbsp; |
    | 403 | Forbidden | &nbsp; |
    | 404 | Not Found | &nbsp; |

    **响应参数**\:

    | 参数名称 | 参数说明 | 类型 | schema |
    | --- | --- | --- | --- |
    | error | &nbsp; | ErrorMessage | ErrorMessage |
    | code | &nbsp; | string | &nbsp; |
    | msg | &nbsp; | string | &nbsp; |
    | msgInfo | &nbsp; | string | &nbsp; |
    | result | &nbsp; | object | &nbsp; |
    | returnCode | &nbsp; | integer(int32) | integer(int32) |
left_code_blocks:
    -
        code_block:
        title: Python
        language: python
right_code_blocks:
    -
        code_block: "\r\n{\r\n\t\"error\": {\r\n\t\t\"code\": \"\",\r\n\t\t\"msg\": \"\"\r\n\t},\r\n\t\"msgInfo\": \"\",\r\n\t\"result\": {},\r\n\t\"returnCode\": 0\r\n}\r\n"
        title: Response
        language: javascript
---
