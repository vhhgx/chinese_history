# 中国历史 CHINESE HISTORY

中国历史JSON数据库

## 皇帝顺序表

暂以下格式为准，后续有扩展再补充


```json
[
  {
    "miao": "庙号",
    "shi": "谥号",
    "supplementary": "布尔值，是否为后世追认",
    "emperorName": "皇帝名讳",
    "birthYear": "生年",
    "deathYear": "卒年",
    "ascendYear": "登基年份",
    "abdicateYear": "退位年份",
    "reignLen": "在位时间",
    "abdicateReason": "退位原因 0: 驾崩（殇），其他需要写明原因",
    "hao": "年号 如果有多个年号则使用数组",
    "年号数组, key依旧为hao": [
      {
        "hao": "年号",
        "startYear": "启用时间",
        "ceaseYear": "停用时间",
        "length": "持续时间"
      }
    ],
    "mausoleum": "皇陵",
    "mausoleumAddress": "皇陵地址",
    "relation": "人物关系"
  }
]
```

## TODO

### 完善

- [ ] 完善历史年表中十六国、南北朝、五代十国数据，并进行校对
- [ ] 完善唐朝皇帝帝陵地址，需要加字段：是否挖掘，挖掘事件
- [ ] 完善唐朝皇帝年号数组
- [ ] 完善明朝皇帝


### 数据结构

- [ ] 突发事件，即位时间短的皇帝。例如哀帝、殇帝，或其他突发事件被迫让位
- [ ] 短暂改朝，例如武瞾改唐为武周
- [ ] 流亡政权，例如南明
- [ ] 后世追认的皇帝，加一个字段用于隐藏
