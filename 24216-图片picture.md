# 图片\_Picture ![](/assets/Picture-icon.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'Image',
    'selected': false,
    'normal': {
        'src': '/public/images/default.png',
        'text': '',
        'imageStyle': {
            'borderRadius': '1px',
            'opacity': '1'
        },
        'textStyle': {
            'color': '#ccc',
            'fontSize': '14px',
            'marginLeft': 0,
            'marginTop': 0
        }
    },
    'mouse': {
        'src': '/public/images/default.png',
        'text': '',
        'imageStyle': {
            'borderRadius': '1px',
            'opacity': '1'
        },
        'textStyle': {
            'color': '#ccc',
            'fontSize': '14px',
            'marginLeft': 0,
            'marginTop': 0
        }
    },
    'emphasis': {
        'src': '/public/images/default.png',
        'text': '',
        'imageStyle': {
            'borderRadius': '1px',
            'opacity': '1'
        },
        'textStyle': {
            'color': '#ccc',
            'fontSize': '14px'
        }
    }
}
```

### 参数字段说明

| Configuration item | Type | Required | Default | Optional parameters | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | Image |  | The only component type |
| selected | Bool | √ | false |  | Whethe the picture is **selected** |
| normal | Object | √ |  |  | The style of **the unselected state** |
| normal.src | String | √ |  |  | The url of **the unselected picture** |
| normal.text | String |  |  |  | The text of **the unselected state** |
| normal.imageStyle | Object | √ |  |  | The style of **the unselected picture** |
| normal.imageStyle.borderRadius | String | √ | 1px |  | The borderRadius of **the unselected picture** |
| normal.imageStyle.opacity | Number | √ | 0.0-1.0 |  | The opacity of **the unselected picture** |
| normal.textStyle | Object | √ |  |  | The style of **the unselected text** |
| normal.textStyle.color | String | √ | \#ccc | The color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent are supported | The color of **the unselected text** |
| normal.textStyle.fontSize | String | √ | 14px |  | The fontSize of **the unselected text** |
| normal.textStyle.marginLeft | String | √ | -21 |  | The marginLeft of **the unselected text** |
| normal.textStyle.marginTop | String | √ | -7 |  | The marginTop of **the unselected text** |
| mouse | Object | √ |  |  | The style of **the hovered **picture by mouse |
| mouse.src | String | √ |  |  | The url of **the hovered picture** |
| mouse.text | String |  |  |  | The text when the picture is **hovered** |
| mouse.imageStyle | Object | √ |  |  | The style of **the hovered picture** |
| mouse.imageStyle.borderRadius | String | √ | 1px |  | The borderRadius of **the hovered picture** |
| mouse.imageStyle.opacity | Number | √ | 0.0-1.0 |  | The opacity of **the hovered picture** |
| mouse.textStyle | Object | √ |  |  | The style of **the hovered text ** |
| mouse.textStyle.color | String | √ | \#ccc | The color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent are supported | The color of **the hovered text** |
| mouse.textStyle.fontSize | String | √ | 14px |  | The fontSize of** the hovered text** |
| mouse.textStyle.marginLeft | String | √ | 0 |  | The marginLeft of **the hovered text** |
| mouse.textStyle.marginTop | String | √ | 0 |  | The marginTop of **the hovered text** |
| emphasis | Object | √ |  |  | The selected picture |
| emphasis.src | String | √ |  |  | The url of **the selected picture** |
| emphasis.text | String |  |  |  | The text when the picture is **selected** |
| emphasis.imageStyle | Object | √ |  |  | The style of** the selected picture** |
| emphasis.imageStyle.borderRadius | String | √ | 1px |  | The borderRadius of **the selected picture** |
| emphasis.imageStyle.opacity | Number | √ | 0.0-1.0 |  | The opacity of the **selected picture** |
| emphasis.textStyle | Object | √ |  |  | The textStyle of the **selected text** |
| emphasis.textStyle.color | String | √ | \#ccc | The color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent are supported | The color of **the selected text** |
| emphasis.textStyle.fontSize | String | √ | 14px |  | The fontSize of the **selected t**ext |

> 注：
>
> * normal.imageStyle和normal.textStyle、mouse.imageStyle和mouse.textStyle、emphasis.imageStyle和emphasis.textStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他图片样式



