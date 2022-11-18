---
title: errorHtml7
position_number: 7
type: post
split: '-------------------------------------'
description: |
    接口地址:/error <br>请求数据类型:application/x-www-form-urlencoded
parameters:
    -
        name: orderId
        type: number
        mandatory: false
        default:
        description: 订单ID
        ranges:
content_markdown: >-
    **响应状态**\:


    | 状态码 | 说明 | schema |

    | --- | --- | --- |

    | 200 | OK | ModelAndView |

    | 204 | No Content | &nbsp; |

    | 401 | Unauthorized | &nbsp; |

    | 403 | Forbidden | &nbsp; |


    **响应参数**\:


    | 参数名称 | 参数说明 | 类型 | schema |

    | --- | --- | --- | --- |

    | empty | &nbsp; | boolean | &nbsp; |

    | model | &nbsp; | object | &nbsp; |

    | modelMap | &nbsp; | object | &nbsp; |

    | reference | &nbsp; | boolean | &nbsp; |

    | status |
    可用值:ACCEPTED,ALREADY\_REPORTED,BAD\_GATEWAY,BAD\_REQUEST,BANDWIDTH\_LIMIT\_EXCEEDED,CHECKPOINT,CONFLICT,CONTINUE,CREATED,DESTINATION\_LOCKED,EXPECTATION\_FAILED,FAILED\_DEPENDENCY,FORBIDDEN,FOUND,GATEWAY\_TIMEOUT,GONE,HTTP\_VERSION\_NOT\_SUPPORTED,IM\_USED,INSUFFICIENT\_SPACE\_ON\_RESOURCE,INSUFFICIENT\_STORAGE,INTERNAL\_SERVER\_ERROR,I\_AM\_A\_TEAPOT,LENGTH\_REQUIRED,LOCKED,LOOP\_DETECTED,METHOD\_FAILURE,METHOD\_NOT\_ALLOWED,MOVED\_PERMANENTLY,MOVED\_TEMPORARILY,MULTIPLE\_CHOICES,MULTI\_STATUS,NETWORK\_AUTHENTICATION\_REQUIRED,NON\_AUTHORITATIVE\_INFORMATION,NOT\_ACCEPTABLE,NOT\_EXTENDED,NOT\_FOUND,NOT\_IMPLEMENTED,NOT\_MODIFIED,NO\_CONTENT,OK,PARTIAL\_CONTENT,PAYLOAD\_TOO\_LARGE,PAYMENT\_REQUIRED,PERMANENT\_REDIRECT,PRECONDITION\_FAILED,PRECONDITION\_REQUIRED,PROCESSING,PROXY\_AUTHENTICATION\_REQUIRED,REQUESTED\_RANGE\_NOT\_SATISFIABLE,REQUEST\_ENTITY\_TOO\_LARGE,REQUEST\_HEADER\_FIELDS\_TOO\_LARGE,REQUEST\_TIMEOUT,REQUEST\_URI\_TOO\_LONG,RESET\_CONTENT,SEE\_OTHER,SERVICE\_UNAVAILABLE,SWITCHING\_PROTOCOLS,TEMPORARY\_REDIRECT,TOO\_EARLY,TOO\_MANY\_REQUESTS,UNAUTHORIZED,UNAVAILABLE\_FOR\_LEGAL\_REASONS,UNPROCESSABLE\_ENTITY,UNSUPPORTED\_MEDIA\_TYPE,UPGRADE\_REQUIRED,URI\_TOO\_LONG,USE\_PROXY,VARIANT\_ALSO\_NEGOTIATES
    | string | &nbsp; |

    | view | &nbsp; | View | View |

    | contentType | &nbsp; | string | &nbsp; |

    | viewName | &nbsp; | string | &nbsp; |


    &nbsp;
left_code_blocks:
    -
        code_block:
        title: Python
        language: python
right_code_blocks:
    -
        code_block: "{\n\t\"empty\": true,\n\t\"model\": {},\n\t\"modelMap\": {},\n\t\"reference\": true,\n\t\"status\": \"\",\n\t\"view\": {\n\t\t\"contentType\": \"\"\n\t},\n\t\"viewName\": \"\"\n}\n"
        title: Response
        language: javascript
---
