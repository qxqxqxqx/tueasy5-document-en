# 菜单\_TreeMenu ![](/assets/TreeMenu.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'treeMenu',
    'series': [
        {
            'name': '北京市',
            'value': 'beijing',
            'childrens': [
                {
                    'name': '朝阳区',
                    'value': 'chaoyangqu',
                    'childrens': [
                        {
                            'name': '朝阳公园',
                            'value': 'chaoyang park'
                        },
                        {
                            'name': '三里屯',
                            'value': 'sanlitun'
                        }
                    ]
                },
                {
                    'name': '海淀区',
                    'value': 'haidianqu'
                }
            ]
        },
        {
            'name': '上海市',
            'value': 'shanghai',
            'childrens': [
                {
                    'name': '徐汇区',
                    'value': 'xuhuiqu'
                },
                {
                    'name': '松江区',
                    'value': 'songjiangqu'
                },
                {
                    'name': '嘉定区',
                    'value': 'jiadingqu'
                }
            ]
        },
        {
            'name': '重庆市',
            'value': 'chongqing',
            'childrens': [
                {
                    'name': '渝北区',
                    'value': 'yubeiqu'
                },
                {
                    'name': '渝中区',
                    'value': 'yuzhongqu'
                },
                {
                    'name': '北碚区',
                    'value': 'beibeiqu'
                }
            ]
        }
    ],
    'titleName': '北京市',
    'SubTreeGap': 30,
    'itemStyle': {
        'primaryStyle': {
            'height': '40px',
            'fontFamily': '微软雅黑',
            'fontSize': '14px',
            'color': '#fff',
            'display': 'inline-block',
            'backgroundColor': 'rgb(102, 118, 136)',
            'lineHeight': '40px'
        },
        'primaryArrowStyle': {
            'fontSize': '18px',
            'color': 'rgb(255, 255, 255)'
        },
        'menuStyle': {
            'normal': {
                'fontSize': '14px',
                'color': '#fff',
                'backgroundColor': 'rgb(102, 118, 136)',
                'fontFamily': '微软雅黑',
                'lineHeight': '30px'
            },
            'emphasis': {
                'color': '#1C243B',
                'backgroundColor': 'rgb(239, 241, 243)'
            }
        }
    }
}
```

### 参数字段说明

| Configuration item | Type | Required | Default | Optional parameters | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | treeMenu |  | Component type, unchangeable |
| series | Array\(Object\) | √ |  |  | Data option of the tree menu, every object item of the array means a level one item |
| series\[0\].name | String | √ |  |  | Text of the menu item, repeated |
| series\[0\].value | String | √ |  |  | Uniquely identification of a menu item |
| series\[0\].children | Object |  |  |  | Child item of this menu item with same constructure |
| titleName | String | √ |  |  | Default text of the menu items, only show when any item is not selected |
| SubTreeGap | String | √ | 30px |  | Right indent between child menu and father menu |
| itemStyle | Object | √ |  |  | Style of menu item |
| itemStyle.primaryStyle | Object | √ |  |  | Primary style of menu item |
| itemStyle.primaryStyle.height | String | √ | 40px | all css3 height parameters | Primary height of menu item |
| itemStyle.primaryStyle.fontFamily | String | √ | 微软雅黑 | all css3 font-family parameters | Primary fontFamily of menu item |
| itemStyle.primaryStyle.fontSize | String | √ | 14px | all css3 font-size parameters | Primary fontSize of menu item |
| itemStyle.primaryStyle.color | String | √ | \#fff | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Primary text color of menu item |
| itemStyle.primaryStyle.display | String | √ | inline-block | all css3 display parameters | Primaty display type of menu text |
| itemStyle.primaryStyle.backgroundColor | String | √ | rgb\(102, 118, 136\) | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Primary background color of menu item |
| itemStyle.primaryStyle.lineHeight | String | √ | 40px | all css3 line-height parameters | Primary line height of menu item |
| itemStyle.primaryArrowStyle | Object | √ |  |  | Primary triangle style of menu item |
| itemStyle.primaryArrowStyle.fontSize | String | √ | 14px | all css3 font-size parameters | Primary triangle size of menu item |
| itemStyle.primaryArrowStyle.color | String | √ | \#fff | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Primary triangle color of menu item |
| itemStyle.menuStyle | Object | √ |  |  | Dropdown style of menu item |
| itemStyle.menuStyle.normal | Object | √ |  |  | **Unselected** style of dropdown menu |
| itemStyle.menuStyle.normal.fontSize | String | √ | 14px | all css3 font-size parameters | **Unselected** fontSize of dropdown menu |
| itemStyle.menuStyle.normal.color | String | √ | \#fff | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Unselected color of dropdown menu |
| itemStyle.menuStyle.normal.backgroundColor | String | √ | rgb\(102, 118, 136\) | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | **Unselected** background color of dropdown menu |
| itemStyle.menuStyle.normal.fontFamily | String | √ | 微软雅黑 | all css3 font-family parameters | **Unselected** fontFamily of dropdown menu |
| itemStyle.menuStyle.normal.lineHeight | String | √ | 40px | all css3 line-height parameters | **Unselected** lineHeight of dropdown menu |
| itemStyle.menuStyle.emphasis | Object | √ |  |  | **Selected** style of dropdown menu |
| itemStyle.menuStyle.emphasis.color | String | √ | \#fff | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | **Selected** text color of dropdown menu |
| itemStyle.menuStyle.emphasis.backgroundColor | String | √ | rgb\(239, 241, 243\) | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | **Selected** background color of dropdown menu |

> 注：
>
> * 菜单尚未绑定数据时，series中的children可以无限嵌套，建议一般三级菜单最号；绑定数据后series会自动生成，用户可根据自己需求手动修该文本内容
> * itemStyle.primaryStyle、itemStyle.primaryArrowStyle、itemStyle.menuStyle.normal和itemStyle.menuStyle.emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他菜单样式



