---
title: handle
position_number: 1
type: get
split: '-------------------------------------'
description: >+
    接口地址:/actuator/health<br>请求数据类型:application/x-www-form-urlencoded,application/json

parameters:
    -
        name: orderId
        type: number
        mandatory: false
        default:
        description: 订单ID
        ranges:
content_markdown: |-
    **响应状态**\:

    | 状态码 | 说明 | schema |
    | --- | --- | --- |
    | 200 | OK | &nbsp; |
    | 401 | Unauthorized | &nbsp; |
    | 403 | Forbidden | &nbsp; |
    | 404 | Not Found | &nbsp; |

    **响应参数**\:

    暂无
left_code_blocks:
    -
        code_block:
        title: Python
        language: python
right_code_blocks:
    -
        code_block: |+

        title: Response
        language: javascript
---
