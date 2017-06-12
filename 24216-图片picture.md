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
| type | String | √ | Image |  | Component type,unchangeable |
| selected | Bool | √ | false |  | Whethe the picture is **selected** |
| normal | Object | √ |  |  | Style of **the unselected state** |
| normal.src | String | √ |  |  | Url of **the unselected picture** |
| normal.text | String |  |  |  | Text of **the unselected state** |
| normal.imageStyle | Object | √ |  |  | Style of **the unselected picture** |
| normal.imageStyle.borderRadius | String | √ | 1px |  | BorderRadius of **the unselected picture** |
| normal.imageStyle.opacity | Number | √ | 0.0-1.0 |  | Opacity of **the unselected picture** |
| normal.textStyle | Object | √ |  |  | Style of **the unselected text** |
| normal.textStyle.color | String | √ | \#ccc | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of **the unselected text** |
| normal.textStyle.fontSize | String | √ | 14px |  | FontSize of **the unselected text** |
| normal.textStyle.marginLeft | String | √ | -21 |  | MarginLeft of **the unselected text** |
| normal.textStyle.marginTop | String | √ | -7 |  | MarginTop of **the unselected text** |
| mouse | Object | √ |  |  | Style of **the hovered **picture by mouse |
| mouse.src | String | √ |  |  | Url of **the hovered picture** |
| mouse.text | String |  |  |  | Content when the picture is **hovered** |
| mouse.imageStyle | Object | √ |  |  | Style of **the hovered picture** |
| mouse.imageStyle.borderRadius | String | √ | 1px |  | BorderRadius of **the hovered picture** |
| mouse.imageStyle.opacity | Number | √ | 0.0-1.0 |  | Opacity of **the hovered picture** |
| mouse.textStyle | Object | √ |  |  | Style of **the hovered text ** |
| mouse.textStyle.color | String | √ | \#ccc | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of **the hovered text** |
| mouse.textStyle.fontSize | String | √ | 14px |  | FontSize of** the hovered text** |
| mouse.textStyle.marginLeft | String | √ | 0 |  | MarginLeft of **the hovered text** |
| mouse.textStyle.marginTop | String | √ | 0 |  | MarginTop of **the hovered text** |
| emphasis | Object | √ |  |  | Selected picture |
| emphasis.src | String | √ |  |  | Url of **the selected picture** |
| emphasis.text | String |  |  |  | Content when the picture is **selected** |
| emphasis.imageStyle | Object | √ |  |  | Style of** the selected picture** |
| emphasis.imageStyle.borderRadius | String | √ | 1px |  | BorderRadius of **the selected picture** |
| emphasis.imageStyle.opacity | Number | √ | 0.0-1.0 |  | Opacity of the **selected picture** |
| emphasis.textStyle | Object | √ |  |  | TextStyle of the **selected text** |
| emphasis.textStyle.color | String | √ | \#ccc | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of **the selected text** |
| emphasis.textStyle.fontSize | String | √ | 14px |  | FontSize of the **selected t**ext |

> 注：
>
> * normal.imageStyle和normal.textStyle、mouse.imageStyle和mouse.textStyle、emphasis.imageStyle和emphasis.textStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他图片样式



