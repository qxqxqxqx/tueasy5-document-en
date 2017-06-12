# 走马灯\_Marquee ![](/assets/Marquee.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'Marquee',
    'series': [
        {
            'date': '2016.9.2',
            'time': '12:28:39',
            'content': '渝北区邮政银行遭遇抢劫'
        },
        {
            'date': '2016.9.2',
            'time': '22:28:39',
            'content': '渝北区珠宝店有小偷进入'
        },
        {
            'date': '2016.9.2',
            'time': '23:28:39',
            'content': '人民大街发生车祸'
        },
        {
            'name': '车辆轨迹',
            'value': 'carInfo'
        },
        {
            'name': '人员密度',
            'value': 'personIdentity'
        },
        {
            'name': '路况',
            'value': 'roadInfo'
        }
    ],
    'categoryGap': '80px',
    'itemGap': '20px',
    'speedTime': 20,
    'speedDistance': '2px',
    'itemStyle': {
        'normal': {
            'fontSize': '20px',
            'color': '#c1c1c1',
            'background': '#eff1f3',
            'paddingLeft': '5px'
        }
    }
}
```

### 参数字段说明

| Configuration item | Type | Required | Default | Optional parameters | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| type | String | √ | Marquee |  | Component type, unchangeable |
| series | Array\(Object\) | √ |  |  | Data of the component |
| series\[0\].name | String | √ |  |  | Uniquely identification of data, unrepeatable |
| series\[0\].value | String | √ |  |  | Content of data, repeatable |
| categoryGap | String | √ | 20px |  | Gap between the bars |
| itemGap | Sting | √ | 10px |  | Gaps between  data items |
| speedTime | Number | √ | 20 |  | Time speed in milliseconds |
| speedDistance | String | √ | 2px |  | Rate |
| itemStyle | Object | √ |  |  | Style of the component |
| itemStyle.normal | Object | √ |  |  | Normal style of the component |
| itemStyle.normal.fontSize | String | √ | 20px | font-size parameters | FontSize of the component |
| itemStyle.normal.color | String | √ | \#c1c1c1 | Color parameters including Color Name、HEX、RGB、RGBA、HSL、HSLA、transparent | Color of the component |
| itemStyle.normal.background | String | √ | \#eff1f3 | all css3 parameters of 'background' | Background style of the component |
| itemStyle.normal.paddingLeft | String | √ | 5px |  | PaddingLeft of the component |

> 注：
>
> * 跑马灯尚未绑定数据时，可以对series\[0\].data进行编辑；跑马灯绑定数据后，series会自动生成相应信息，可根据相应需求进行数据改动
> * 跑马灯的滑动速率由speedTime和speedDistance决定，单位时间内\(speedTime\)跑马灯走过的像素\(speedDistance\)
> * itemStyle.normal中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他跑马灯样式
> * 对于categoryGap和itemGap的区别如下图所示：

![](/assets/marquee01.png)

