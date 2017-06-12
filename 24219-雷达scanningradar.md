# 雷达\_ScanningRadar ![](/assets/ScanningRadar.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'scanningRadar': {
        'splitLine': {
            'show': true,
            'lineStyle': {
                'stroke': '#0afea4'
            }
        },
        'axisLine': {
            'show': true,
            'lineStyle': {
                'stroke': '#0afea4'
            }
        }
    },
    'series': [
        {
            'type': 'scanningRadar',
            'colors': [
                'white',
                '#10a7ba',
                'white'
            ]
        }
    ]
}
```

### 参数字段说明

| Configuration item | Type | Required | Default | Optional parameters | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| scanningRadar | Object | √ |  |  | Background style of the radar |
| scanningRadar.splitLine | Object | √ |  |  | Ring style of the radar background |
| scanningRadar.splitLine.show | Bool | √ | true |  | Whether or not to show the ring |
| scanningRadar.splitLine.lineStyle | Object | √ |  |  | Line style of the ring |
| scanningRadar.splitLine.lineStyle.stroke | String | √ | \#0afea4 |  | Color of the ring |
| scanningRadar.axisLine | Object |  |  |  | Axis line of the radar |
| scanningRadar.axisLine.show | Bool | √ | true |  | Whether or not to show axis line |
| scanningRadar.axisLine.lineStyle | Object | √ |  |  | Style of axis line |
| scanningRadar.axisLine.lineStyle.stroke | String | √ | \#0afea4 |  | Color of axis line |
| series | Array\(Object\) | √ |  |  | Color matching of scanning part |
| series\[0\].type | String | √ | scanningRadar |  | Component type, unchangeable |
| series\[0\].colors | String | √ | 'white','\#10a7ba','white' |  | Color group of scanning part |



