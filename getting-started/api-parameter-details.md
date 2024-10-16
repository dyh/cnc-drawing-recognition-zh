# 接口参数详细信息

## 数控图纸识别接口

## <mark style="color:green;">`POST`</mark> [`http://api.holdingsky.cn/v1/tuzhi`](http://api.holdingsky.cn/v1/tuzhi)



**POST 内容**

| 名称     | 类型   | 描述                                |
| ------ | ---- | --------------------------------- |
| `file` | file | <p>支持的文件格式：</p><p>pdf、jpg、png</p> |

**POST 响应**

{% tabs %}
{% tab title="200" %}
```json
{
    "ban_mian_fen_xi":
    [
        {
            "版面分析结果可视化图片": "http://192.168.2.24:19096/static/banmian_output_det/1727164869.5096982.jpg",
            "页码": 1
        }
    ],
    "guan_jian_chi_cun_xin_xi":
    [
        {
            "上偏差": "+0.5",
            "下偏差": "-0.5",
            "位置":
            [
                0.47987117552334946,
                0.4416184971098266,
                0.5209339774557166,
                0.45895953757225433
            ],
            "基准": "M3",
            "尺寸类型": "",
            "数量": "",
            "最大值": "",
            "最小值": "",
            "置信度": 0.79052734375,
            "页码": 1
        },
        {
            "上偏差": "+0.03",
            "下偏差": "0",
            "位置":
            [
                0.05636070853462158,
                0.2323699421965318,
                0.07246376811594203,
                0.2809248554913295
            ],
            "基准": "13",
            "尺寸类型": "",
            "数量": "",
            "最大值": "",
            "最小值": "",
            "置信度": 0.7958984375,
            "页码": 1
        }
    ],
    "xing_wei_gong_cha":
    [
        {
            "位置":
            [
                0.5491143317230274,
                0.2520231213872832,
                0.5668276972624798,
                0.3491329479768786
            ],
            "实体要求": "",
            "实体要求1": "",
            "实体要求2": "",
            "实体要求3": "",
            "尺寸类型": "",
            "形位公差值": "0.02",
            "形位公差基准1": "C",
            "形位公差基准2": "",
            "形位公差基准3": "",
            "置信度": 0.93701171875,
            "页码": 1,
            "项目特征": "同轴(同心)度"
        },
        {
            "位置":
            [
                0.3711755233494364,
                0.3202312138728324,
                0.44122383252818037,
                0.34566473988439306
            ],
            "实体要求": "",
            "实体要求1": "",
            "实体要求2": "",
            "实体要求3": "",
            "尺寸类型": "",
            "形位公差值": "0.02",
            "形位公差基准1": "B",
            "形位公差基准2": "",
            "形位公差基准3": "",
            "置信度": 0.9462890625,
            "页码": 1,
            "项目特征": "平行度"
        }
    ],
    "notes":
    [
        [
            {
                "位置": "",
                "内容": "1.材料：AZ91D",
                "出现次数": 0,
                "字段位置":
                [
                    0.07889309313597169,
                    0.7674659244986798,
                    0.15921007750093208,
                    0.783550988367944
                ],
                "属性":
                {
                    "材料":
                    [
                        {
                            "材料": "材料"
                        },
                        {
                            "材料": "AZ91D"
                        },
                        {
                            "材料规范": "AZ91D"
                        }
                    ]
                },
                "序号": ""
            },
            {
                "位置": "",
                "内容": "表面处理：本色，表面喷沙/波化",
                "出现次数": 0,
                "字段位置":
                [
                    0.08612162172881813,
                    0.7824020552344252,
                    0.2571967984261837,
                    0.8007849853707272
                ],
                "属性":
                {
                    "硫阳本色":
                    [
                        {
                            "硫阳本色": "本色"
                        }
                    ]
                },
                "序号": ""
            },
            {
                "位置": "",
                "内容": "2.a.未注公差按上标列表：",
                "出现次数": 0,
                "字段位置":
                [
                    0.07969626297962129,
                    0.8007849853707272,
                    0.2098097776508571,
                    0.8180189823735103
                ],
                "属性":
                {
                    "未注规范":
                    [
                        {
                            "未注规范": "未注公差"
                        }
                    ]
                },
                "序号": ""
            },
            {
                "位置": "",
                "内容": "角度公差+/-0.5度.",
                "出现次数": 0,
                "字段位置":
                [
                    0.1029881884454598,
                    0.8352529793762935,
                    0.20177807921436108,
                    0.8524869763790766
                ],
                "属性":
                {
                    "公差要求":
                    [
                        {
                            "公差要求": "+/-0.5度"
                        }
                    ]
                },
                "序号": ""
            },
            {
                "位置": "",
                "内容": "3.零件材质必须符合ROHS、REACH、CP65、欧美环保要求．",
                "出现次数": 0,
                "字段位置":
                [
                    0.07969626297962129,
                    0.8869549703846429,
                    0.3977515210648644,
                    0.9041889673874259
                ],
                "属性":
                {
                    "材料":
                    [
                        {
                            "材料": "材质"
                        },
                        {
                            "材料规范": "ROHS、REACH、CP65、欧美环保"
                        }
                    ]
                },
                "序号": ""
            }
        ]
    ],
    "ji_chu_xin_xi":
    [
        {
            "ANGLES": "",
            "FINISH": "",
            "STATUS": "",
            "位置":
            [
                0.6731078904991948,
                0.8439306358381503,
                0.9718196457326892,
                0.9514450867052023
            ],
            "公差": "",
            "关键件": "否",
            "图号": "",
            "审核人": "",
            "审核时间": "",
            "尺寸单位": "",
            "批准人": "",
            "批准时间": "",
            "数量": "",
            "未注粗糙度": "",
            "材料": "",
            "版本": "",
            "置信度": 0.94921875,
            "角向信息": "角向一",
            "设计人": "",
            "设计时间": "",
            "重量": "",
            "零件名称": ""
        }
    ],
    "ji_zhun":
    [
        {
            "位置":
            [
                0.5668276972624798,
                0.27976878612716766,
                0.5805152979066023,
                0.2994219653179191
            ],
            "基准值": "M",
            "页码": 1
        },
        {
            "位置":
            [
                0.2616747181964573,
                0.14219653179190753,
                0.2777777777777778,
                0.1791907514450867
            ],
            "基准值": "A",
            "页码": 1
        },
        {
            "位置":
            [
                0.2431561996779388,
                0.2728323699421965,
                0.25925925925925924,
                0.30982658959537573
            ],
            "基准值": "B",
            "页码": 1
        },
        {
            "位置":
            [
                0.4919484702093398,
                0.3283236994219653,
                0.5169082125603864,
                0.353757225433526
            ],
            "基准值": "C",
            "页码": 1
        }
    ],
    "bom_biaoshi":
    [
        {
            "位置":
            [
                0.4895330112721417,
                0.45664739884393063,
                0.5024154589371981,
                0.47398843930635837
            ],
            "内容": "23",
            "置信度": 0.85107421875,
            "页码": 1
        }
        {
            "位置":
            [
                0.32930756843800324,
                0.15953757225433526,
                0.34299516908212563,
                0.1791907514450867
            ],
            "内容": "34",
            "置信度": 0.88232421875,
            "页码": 1
        }
    ],
    "lingjian_2d":
    [
        {
            "位置":
            [
                0.710950080515298,
                0.33410404624277457,
                0.9331723027375202,
                0.5942196531791908
            ],
            "置信度": 0.8251953125,
            "页码": 1
        },
        {
            "位置":
            [
                0.5273752012882448,
                0.3329479768786127,
                0.6400966183574879,
                0.5965317919075145
            ],
            "置信度": 0.861328125,
            "页码": 1
        }
    ],
    "lingjian_3d":
    [
        {
            "位置":
            [
                0.8293075684380032,
                0.6809248554913295,
                0.962157809983897,
                0.8277456647398844
            ],
            "置信度": 0.9716796875,
            "页码": 1
        }
    ]
}
```
{% endtab %}

{% tab title="400" %}
```json
{
  "error": "Invalid request"
}
```
{% endtab %}
{% endtabs %}

