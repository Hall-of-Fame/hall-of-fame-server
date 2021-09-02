## `GET /departments`

### Description

返回各个分部门的图片信息。

### Response

返回格式为 JSON，参考以下示例：

```json5
[
    {
        "name": "PM",
        "grades": [
            /* ... */
        ]
    },
    {
        "name": "Design",
        "grades": [
            /* ... */
        ]
    },
    {
        "name": "Frontend",
        "grades": [
            /* ... */
        ]
    },
    {
        "name": "Backend",
        "grades": [
            {
                "name": "20",
                "students": [
                    /* ... */
                    {
                        "name": "吴昊达",
                        "avatar": "114514",
                        "stickers": [
                            {
                                "desc": "我是霸道总裁",
                                "url": "/static/Backend/20/吴昊达/我是霸道总裁.jpeg"
                            },
                        ]
                    }
                ]
            },
            /* ... */
        ]
    },
    {
        "name": "Android",
        "grades": [
            /* ... */
        ]
    },
    {
        "name": "iOS",
        "grades": [
            /* ... */
        ]
    },
    {
        "name": "SRE",
        "grades": [
            /* ... */
        ]
    },
    {
        "name": "0xfa",
        "grades": [
            /* ... */
        ]
    }
]
```


## `GET /multiple` (UNCOMPLETED)

### Description

返回图片中同时含有多人对话的所有图片。

### Response

返回格式为 JSON，`author` 一般采用缩写（顺便整活儿），参考一下示例：

```json5
[
    /* ... */
    {
        // 冯宇祥，黄凯升，吴昊达
        "author": "冯凯达",
        "title": "发生甚么事了-是我想你了",
        "url": "/static/other/冯凯达-发生甚么事了-我想你了.jpg"
    }, {
        // 郭祥瑞，王兮
        "author": "祥兮",
        "title": "只要你想 你也可以成为学姐-我一直在想",
        "url": "/static/other/祥兮-只要你想％20你也可以成为学姐-我一直在想.jpg"
    }, {
        // 黄凯升，路明瑞
        "author": "黄瑞",
        "title": "🏳️‍🌈 🏳️‍⚧️ LGBTQ LIVES MATTER!",
        "url": "/static/other/黄瑞-🏳️‍🌈％20🏳️‍⚧️％20LGBTQ％20LIVES％20MATTER!.jpg"
    }
]
```