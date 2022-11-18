---
title: Get depth data
position_number: 3
type: get
split: '-------------------------------------'
description: /v4/public/depth
parameters:
    -
        name: symbol
        type: string
        mandatory: true
        default:
        description: trading pair  eg:btc_usdt
        ranges:
    -
        name: limit
        type: number
        mandatory: false
        default: '50'
        description:
        ranges: 1~500
content_markdown: |-
    #### **Limit Flow Rules**

    200/s/ip
left_code_blocks:
    -
        code_block: |-
            public String depth(){


            }
        title: Java
        language: java
    -
        code_block:
        title: Python
        language: python
right_code_blocks:
    -
        code_block: |-
            {
              "rc": 0,
              "mc": "SUCCESS",
              "ma": [],
              "result": {
                "timestamp": 1662445330524,  
                "lastUpdateId": 137333589606963580,     //Last updated record
                "bids": [                               //buy order([?][0]=price;[?][1]=pending order volume)
                  [
                    "200.0000",                         //price
                    "0.996000"                          //pending order volume
                  ],
                  [
                    "100.0000",
                    "0.001000"
                  ],
                  [
                    "20.0000",
                    "10.000000"
                  ]
                ],
                "asks": []                              //sell order([?][0]=price;[?][1]=pending order volume)
              }
            }
        title: Response
        language: json
---
\#\# errorHtml

<br>\*\*接口地址\*\*:\`/error\`

<br>\*\*请求方式\*\*:\`GET\`

<br>\*\*请求数据类型\*\*:\`application/x-www-form-urlencoded\`

<br>\*\*响应数据类型\*\*:\`\*/\*\`

<br>\*\*接口描述\*\*:

<br>\*\*请求参数\*\*:

<br>\*\*请求参数\*\*:

<br>暂无

<br>\*\*响应状态\*\*:

<br>\| 状态码 \| 说明 \| schema \|<br>\| -------- \| -------- \| ----- \|&nbsp;<br>\|200\|OK\|ModelAndView\|<br>\|401\|Unauthorized\|\|<br>\|403\|Forbidden\|\|<br>\|404\|Not Found\|\|

<br>\*\*响应参数\*\*:

<br>\| 参数名称 \| 参数说明 \| 类型 \| schema \|<br>\| -------- \| -------- \| ----- \|----- \|&nbsp;<br>\|empty\|\|boolean\|\|<br>\|model\|\|object\|\|<br>\|modelMap\|\|object\|\|<br>\|reference\|\|boolean\|\|<br>\|status\|可用值:ACCEPTED,ALREADY\_REPORTED,BAD\_GATEWAY,BAD\_REQUEST,BANDWIDTH\_LIMIT\_EXCEEDED,CHECKPOINT,CONFLICT,CONTINUE,CREATED,DESTINATION\_LOCKED,EXPECTATION\_FAILED,FAILED\_DEPENDENCY,FORBIDDEN,FOUND,GATEWAY\_TIMEOUT,GONE,HTTP\_VERSION\_NOT\_SUPPORTED,IM\_USED,INSUFFICIENT\_SPACE\_ON\_RESOURCE,INSUFFICIENT\_STORAGE,INTERNAL\_SERVER\_ERROR,I\_AM\_A\_TEAPOT,LENGTH\_REQUIRED,LOCKED,LOOP\_DETECTED,METHOD\_FAILURE,METHOD\_NOT\_ALLOWED,MOVED\_PERMANENTLY,MOVED\_TEMPORARILY,MULTIPLE\_CHOICES,MULTI\_STATUS,NETWORK\_AUTHENTICATION\_REQUIRED,NON\_AUTHORITATIVE\_INFORMATION,NOT\_ACCEPTABLE,NOT\_EXTENDED,NOT\_FOUND,NOT\_IMPLEMENTED,NOT\_MODIFIED,NO\_CONTENT,OK,PARTIAL\_CONTENT,PAYLOAD\_TOO\_LARGE,PAYMENT\_REQUIRED,PERMANENT\_REDIRECT,PRECONDITION\_FAILED,PRECONDITION\_REQUIRED,PROCESSING,PROXY\_AUTHENTICATION\_REQUIRED,REQUESTED\_RANGE\_NOT\_SATISFIABLE,REQUEST\_ENTITY\_TOO\_LARGE,REQUEST\_HEADER\_FIELDS\_TOO\_LARGE,REQUEST\_TIMEOUT,REQUEST\_URI\_TOO\_LONG,RESET\_CONTENT,SEE\_OTHER,SERVICE\_UNAVAILABLE,SWITCHING\_PROTOCOLS,TEMPORARY\_REDIRECT,TOO\_EARLY,TOO\_MANY\_REQUESTS,UNAUTHORIZED,UNAVAILABLE\_FOR\_LEGAL\_REASONS,UNPROCESSABLE\_ENTITY,UNSUPPORTED\_MEDIA\_TYPE,UPGRADE\_REQUIRED,URI\_TOO\_LONG,USE\_PROXY,VARIANT\_ALSO\_NEGOTIATES\|string\|\|<br>\|view\|\|View\|View\|<br>\|&amp;emsp;&amp;emsp;contentType\|\|string\|\|<br>\|viewName\|\|string\|\|

<br>\*\*响应示例\*\*:<br>\`\`\`javascript<br>\{<br>&nbsp;&nbsp; &nbsp;"empty": true,<br>&nbsp;&nbsp; &nbsp;"model": \{\},<br>&nbsp;&nbsp; &nbsp;"modelMap": \{\},<br>&nbsp;&nbsp; &nbsp;"reference": true,<br>&nbsp;&nbsp; &nbsp;"status": "",<br>&nbsp;&nbsp; &nbsp;"view": \{<br>&nbsp;&nbsp; &nbsp; &nbsp; &nbsp;"contentType": ""<br>&nbsp;&nbsp; &nbsp;\},<br>&nbsp;&nbsp; &nbsp;"viewName": ""<br>\}<br>\`\`\`