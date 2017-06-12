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
| themeColor | String | √ | \#667688 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Theme color of calendar page |
| orient | String | √ | vertical | horizontal、vertical | Whether to show the calender horizontally or vertically |
| inputStyle | Object | √ |  |  | Style of input field |
| inputStyle.color | String | √ | \#333 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Text color of input field |
| inputStyle.fontSize | String | √ | 18px | All css3 parameters about fontSize | FontSize of input field |
| inputStyle.fontFamily | String | √ | simsun | All css3 parameters about fontFamily | FontFamily of input field |
| buttonStyle | Object | √ |  |  | Style of confirm button |
| buttonStyle.normal | Object | √ |  |  | **Normal style **of confirm button |
| buttonStyle.normal.backgroundColor | String | √ | \#33b26e | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | **Normal background colo**r of confirm button |
| buttonStyle.normal.color | String | √ | white | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | **Normal text colo**r of confirm button |
| buttonStyle.normal.fontSize | String | √ | 18px | All css3 parameters about fontSize | **Normal fontSize** of confirm button |
| buttonStyle.normal.width | String | √ | 100px | All css3 parameters about width | **Normal width** of confirm button |
| buttonStyle.emphsis | String | √ | 微软雅黑 | All css3 parameters about fontFamily | Style when confirm button is **hovered** |
| buttonStyle.emphsis.backgroundColor | String | √ | violet | All css3 parameters about fontSize | Background color when confirm button is **hovered** |
| buttonStyle.emphsis.color | String | √ | cyan | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Text color when confirm button is **hovered** |
| buttonStyle.emphsis.fontSize | String | √ | 18px | All css3 parameters about fontSize | FontSize when confirm button is **hovered** |

> 注：
>
> * inputStyle和buttonStyle.normal、buttonStyle.emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他日历样式



