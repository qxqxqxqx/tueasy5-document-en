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
| type | String | √ | treeMenu |  | The only component type is treeMenu |
| series | Array\(Object\) | √ |  |  | Data option of the tree menu, every object item of the array means a level one item |
| series\[0\].name | String | √ |  |  | Text of the menu item, repeated |
| series\[0\].value | String | √ |  |  | Uniquely identification of a menu item |
| series\[0\].children | Object |  |  |  | Child item of this menu item with same constructure |
| titleName | String | √ |  |  | 初始化菜单时的默认菜单项文本内容。仅用于初始化显示，未选中当前任何菜单项 |
| SubTreeGap | String | √ | 30px |  | 子菜单距离父级菜单向右缩进的距离 |
| itemStyle | Object | √ |  |  | 菜单项的样式 |
| itemStyle.primaryStyle | Object | √ |  |  | 菜单项显示栏的样式 |
| itemStyle.primaryStyle.height | String | √ | 40px | 支持CSS3中height的参数值 | 菜单项显示栏的高度 |
| itemStyle.primaryStyle.fontFamily | String | √ | 微软雅黑 | 支持CSS3中font-family的参数值 | 菜单项显示栏的文本样式 |
| itemStyle.primaryStyle.fontSize | String | √ | 14px | 支持CSS3中font-size的参数值 | 菜单项显示栏的文本大小 |
| itemStyle.primaryStyle.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 菜单项显示栏的文本颜色 |
| itemStyle.primaryStyle.display | String | √ | inline-block | 支持CSS3中display的参数值 | 菜单项显示栏的文本显示 |
| itemStyle.primaryStyle.backgroundColor | String | √ | rgb\(102, 118, 136\) | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 菜单项显示栏的背景颜色 |
| itemStyle.primaryStyle.lineHeight | String | √ | 40px | 支持CSS3中line-height的参数值 | 菜单项显示栏的文本行间距 |
| itemStyle.primaryArrowStyle | Object | √ |  |  | 菜单项显示栏的三角标样式 |
| itemStyle.primaryArrowStyle.fontSize | String | √ | 14px | 支持CSS3中font-size的参数值 | 菜单项显示栏的三角标大小 |
| itemStyle.primaryArrowStyle.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 菜单项显示栏的三角标颜色 |
| itemStyle.menuStyle | Object | √ |  |  | 菜单项下拉菜单的样式 |
| itemStyle.menuStyle.normal | Object | √ |  |  | 下拉菜单**未选中**状态样式 |
| itemStyle.menuStyle.normal.fontSize | String | √ | 14px | 支持CSS3中font-size的参数值 | 下拉菜单**未选中**状态的文本大小 |
| itemStyle.menuStyle.normal.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 下拉菜单**未选中**状态的文本颜色 |
| itemStyle.menuStyle.normal.backgroundColor | String | √ | rgb\(102, 118, 136\) | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 下拉菜单**未选中**状态的背景颜色 |
| itemStyle.menuStyle.normal.fontFamily | String | √ | 微软雅黑 | 支持CSS3中font-family的参数值 | 下拉菜单**未选中**状态的文本样式 |
| itemStyle.menuStyle.normal.lineHeight | String | √ | 40px | 支持CSS3中line-height的参数值 | 下拉菜单**未选中**状态的文本行间距 |
| itemStyle.menuStyle.emphasis | Object | √ |  |  | 下拉菜单**选中**状态样式 |
| itemStyle.menuStyle.emphasis.color | String | √ | \#fff | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 下拉菜单**选中**状态的文本颜色 |
| itemStyle.menuStyle.emphasis.backgroundColor | String | √ | rgb\(239, 241, 243\) | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | 下拉菜单**选中**状态的背景颜色 |

> 注：
>
> * 菜单尚未绑定数据时，series中的children可以无限嵌套，建议一般三级菜单最号；绑定数据后series会自动生成，用户可根据自己需求手动修该文本内容
> * itemStyle.primaryStyle、itemStyle.primaryArrowStyle、itemStyle.menuStyle.normal和itemStyle.menuStyle.emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他菜单样式



