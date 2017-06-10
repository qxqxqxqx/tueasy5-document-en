# 时间\_MultiCalendar ![](/assets/MultiCalendar.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'multiCalendar',
    'themeColor': '#667688',
    'orient': 'vertical',
    'inputStyle': {
        'color': '#333',
        'fontSize': '20px',
        'fontFamily': 'simsun'
    },
    'buttonStyle': {
        'normal': {
            'backgroundColor': '#33b26e',
            'color': 'white',
            'fontSize': '18px',
            'width': '100px'
        },
        'emphsis': {
            'backgroundColor': 'violet',
            'color': 'cyan',
            'fontSize': '18px'
        }
    }
}
```

### 参数字段说明

| Configuration item | Type | Required | Default | Optional parameters | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | multiCalendar |  | The only component type is multiCalendar |
| themeColor | String | √ | \#667688 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 日历界面的主体颜色 |
| orient | String | √ | vertical | horizontal、vertical | 日历展示方式。horizontal横向展示、vertical纵向展示 |
| inputStyle | Object | √ |  |  | 日期显示框的样式 |
| inputStyle.color | String | √ | \#333 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 日期显示框文本颜色 |
| inputStyle.fontSize | String | √ | 18px | 支持CSS3中font-size的参数值 | 日期显示框文本大小 |
| inputStyle.fontFamily | String | √ | simsun | 支持CSS3中font-family的参数值 | 日期显示框文本样式 |
| buttonStyle | Object | √ |  |  | 确认按钮样式 |
| buttonStyle.normal | Object | √ |  |  | 确认按钮**普通**状态样式 |
| buttonStyle.normal.backgroundColor | String | √ | \#33b26e | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 确认按钮**普通**背景颜色 |
| buttonStyle.normal.color | String | √ | white | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 确认按钮**普通**状态文本颜色 |
| buttonStyle.normal.fontSize | String | √ | 18px | 支持CSS3中font-size的参数值 | 确认按钮**普通**状态文本大小 |
| buttonStyle.normal.width | String | √ | 100px | 支持CSS3中width的参数值 | 确认按钮**普通**状态宽度 |
| buttonStyle.emphsis | String | √ | 微软雅黑 | 支持CSS3中font-family的参数值 | 确认按钮**鼠标悬浮**状态样式 |
| buttonStyle.emphsis.backgroundColor | String | √ | violet | 支持CSS3中font-size的参数值 | 确认按钮**鼠标悬浮**状态文本大小 |
| buttonStyle.emphsis.color | String | √ | cyan | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 确认按钮**鼠标悬浮**状态文本颜色 |
| buttonStyle.emphsis.fontSize | String | √ | 18px | 支持CSS3中font-size的参数值 | 确认按钮**鼠标悬浮**状态文本大小 |

> 注：
>
> * inputStyle和buttonStyle.normal、buttonStyle.emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他日历样式



