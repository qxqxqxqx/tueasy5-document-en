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
| themeColor | String | √ | \#667688 | The color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent are supported | The theme color of the calendar page |
| orient | String | √ | vertical | horizontal、vertical | Whether to show the calender horizontally or vertically |
| inputStyle | Object | √ |  |  | The style of the input |
| inputStyle.color | String | √ | \#333 | The color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent are supported | The text color of the input |
| inputStyle.fontSize | String | √ | 18px | All css3 parameters about fontSize | The fontSize of the input |
| inputStyle.fontFamily | String | √ | simsun | All css3 parameters about fontFamily | The fontFamily of the input |
| buttonStyle | Object | √ |  |  | The style of the confirm button |
| buttonStyle.normal | Object | √ |  |  | The **normal style **of the confirm button |
| buttonStyle.normal.backgroundColor | String | √ | \#33b26e | The color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent are supported | The **normal background colo**r of the confirm button |
| buttonStyle.normal.color | String | √ | white | The color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent are supported | The** normal text colo**r of the confirm button |
| buttonStyle.normal.fontSize | String | √ | 18px | All css3 parameters about fontSize | The **normal fontSize** of the confirm button |
| buttonStyle.normal.width | String | √ | 100px | All css3 parameters about width | The **normal width** of the confirm button |
| buttonStyle.emphsis | String | √ | 微软雅黑 | All css3 parameters about fontFamily | The style when the confirm button is **hovered** |
| buttonStyle.emphsis.backgroundColor | String | √ | violet | All css3 parameters about fontSize | The background color when the confirm button is **hovered** |
| buttonStyle.emphsis.color | String | √ | cyan | The color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent are supported | The text color when the confirm button is **hovered** |
| buttonStyle.emphsis.fontSize | String | √ | 18px | All css3 parameters about fontSize | The fontSize when the confirm button is **hovered** |

> 注：
>
> * inputStyle和buttonStyle.normal、buttonStyle.emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他日历样式



