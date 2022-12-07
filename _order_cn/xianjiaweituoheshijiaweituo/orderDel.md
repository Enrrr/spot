---
title: 批量下单
position_number: 1
type: post
split: '-------------------------------------'
description: |
    接口地址:/v1/trade/order/batchOrder <br>请求数据类型:application/x-www-form-urlencoded
content_markdown: >-
    **请求参数**\:


    | 参数名称 | 参数说明 | 请求类型 | 是否必须 | 数据类型 | schema |

    | --- | --- | --- | --- | --- | --- |

    | list | 参数组 | query | true | string | &nbsp; |


    list示例\[\{"symbol":"BTC\_USDT","price":1234,"totalAmount":10,"tradeType":"LIMIT","direction":"BUY"\},\{"symbol":"BTC\_USDT","price":1234,"totalAmount":10,"tradeType":"LIMIT","direction":"BUY"\}\]


    **响应状态**\:


    | 状态码 | 说明 | schema |

    | --- | --- | --- |

    | 200 | OK | CommonResponse&laquo;boolean&raquo; |

    | 201 | Created | &nbsp; |

    | 401 | Unauthorized | &nbsp; |

    | 403 | Forbidden | &nbsp; |

    | 404 | Not Found | &nbsp; |


    **响应参数**\:


    | 参数名称 | 参数说明 | 类型 | schema |

    | --- | --- | --- | --- |

    | code | &nbsp; | integer(int32) | integer(int32) |

    | data | &nbsp; | boolean | &nbsp; |

    | msg | &nbsp; | string | &nbsp; |


    &nbsp;
left_code_blocks:
    -
        code_block:
        title: Python
        language: python
right_code_blocks:
    -
        code_block: "{\n\t\"code\": 0,\n\t\"data\": true,\n\t\"msg\": \"\"\n}\n"
        title: Response
        language: javascript
---
