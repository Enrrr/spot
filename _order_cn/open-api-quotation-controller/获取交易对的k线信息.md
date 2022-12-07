---
title: 获取交易对的k线信息
position_number: 3
type: get
split: '-------------------------------------'
description: |
    接口地址:/v1/q/kline<br>请求数据类型:application/x-www-form-urlencoded
content_markdown: >-
    **请求参数**\:


    | 参数名称 | 参数说明 | 请求类型 | 是否必须 | 数据类型 | schema |

    | --- | --- | --- | --- | --- | --- |

    | interval | 时间间隔(15m 30m 1h 4h 6h 12h 1d 1w) | query | true | string |
    &nbsp; |

    | symbol | 交易对(BTC\_USDT) | query | true | string | &nbsp; |

    | endTime | 结束时间(1670387918970) | query | false | integer(int64) | &nbsp; |

    | limit | 限制条数 | query | false | integer(int32) | &nbsp; |

    | startTime | 起始时间 | query | false | integer(int64) | &nbsp; |


    **响应状态**\:


    | 状态码 | 说明 | schema |

    | --- | --- | --- |

    | 200 | OK | CommonResponse&laquo;List&laquo;KlineVO&raquo;&raquo; |

    | 401 | Unauthorized | &nbsp; |

    | 403 | Forbidden | &nbsp; |

    | 404 | Not Found | &nbsp; |


    **响应参数**\:


    | 参数名称 | 参数说明 | 类型 | schema |

    | --- | --- | --- | --- |

    | code | &nbsp; | integer(int32) | integer(int32) |

    | data | &nbsp; | array | KlineVO |

    | a | 成交量 | number(bigdecimal) | &nbsp; |

    | c | 结束价 | number(bigdecimal) | &nbsp; |

    | h | 最高价 | number(bigdecimal) | &nbsp; |

    | l | 最低价 | number(bigdecimal) | &nbsp; |

    | o | 开始价 | number(bigdecimal) | &nbsp; |

    | s | 交易对 | string | &nbsp; |

    | t | 时间 | integer(int64) | &nbsp; |

    | v | 成交额 | number(bigdecimal) | &nbsp; |

    | msg | &nbsp; | string | &nbsp; |


    &nbsp;
left_code_blocks:
    -
        code_block:
        title: Python
        language: python
right_code_blocks:
    -
        code_block: "{\n\t\"code\": 0,\n\t\"data\": [\n\t\t{\n\t\t\t\"a\": 0,\n\t\t\t\"c\": 0,\n\t\t\t\"h\": 0,\n\t\t\t\"l\": 0,\n\t\t\t\"o\": 0,\n\t\t\t\"s\": \"\",\n\t\t\t\"t\": 0,\n\t\t\t\"v\": 0\n\t\t}\n\t],\n\t\"msg\": \"\"\n}"
        title: Response
        language: javascript
---
