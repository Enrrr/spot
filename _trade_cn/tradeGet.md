---
title: 完整ticker
position_number: 7
type: get
description: /v4/public/ticker
parameters:
    -
        name: symbol
        type: string
        mandatory: false
        default:
        description: 交易对  eg:btc_usdt
        ranges:
    -
        name: symbols
        type: array
        mandatory: false
        default:
        description: '交易对集合，优先级高于symbol。 eg: btc_usdt,eth_usdt'
        ranges:
    -
        name: tags
        type: string
        mandatory: false
        default:
        description: '标签集合,逗号分割，当前仅支持 spot'
        ranges:
content_markdown: >-
    #### **测试**


    1\.毛蛋：100/s/ip


    2\.多个交易对：10/s/ip


left_code_blocks:
    -
        code_block: |-
            public String price(){


            }
        title: bibi
        language: java
    -
        code_block:
        title: 百度
        language: python
right_code_blocks:
    -
        code_block: |-
            {
              "empty": true,
              "model": {},
              "modelMap": {},
              "reference": true,
              "status": "",
              "view": {
                "contentType": ""
              },
              "viewName": ""
            }
        title: 测试
        language: json
---
