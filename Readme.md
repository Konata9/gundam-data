# 高达台词数据库(gundam-lines-database)

[![license](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/0079-104-blue.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/Z-preparing-green.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/0093-preparing-green.svg?style=flat-square)]()

[English](./Readme_en.md)

[日本語](./Readme_jp.md)

## 目的
这个库是我在做"夏亚名台词"系列（发表在微信个人公众号上）的副产物。目前收录了夏亚在《高达0079》中的经典台词，共104句。包含了日语原文、中文翻译、出自人物以及出自话数。日语台词数据来自于互联网。

**注：** 中文翻译为自己翻译，由于水平有限，难免会有错误发生。若发现任何问题可在 issue 中与我交流。

在搜集数据时，发现高达的名言虽然很多，但没有一个很集中的地方。如同星星点点散落在大海那样。于是便有了在搜集整理完成后做成公开数据库的想法，希望可以帮助到同样喜欢高达的人们。你可以利用这些数据做任何有益的事情。也可以提供想法大家一起开发。

## 数据结构
数据分为 JSON 和 sql 两种格式。两种格式字段内容相同。文件采用 Navicat 导出，因此也可以使用 Navicat 导入。根据自己的需要编辑字段。

**文件命名**

gundam_lines_系列名_出自人物（罗马音）.json/sql

**字段含义**

编号 | 字段 | 含义
---- | ----- | ---- 
1 | id | MySQL 主键 id 
2 | order | 语句顺序
3 | line | 台词中文翻译
4 | line_jp | 台词日语原文
5 | series | 高达系列 
6 | episode | 出自话数
7 | person | 出自角色中文翻译
8 | person_jp | 出自角色日语原文

**JSON数据展示**
```json
...
  {
    "id": 1,
    "order": 1,
    "line": "我还真是个不走运的男人啊。在作战结束返航的路上，竟然遇到这等的猎物。",
    "line_jp": "私もよくよく運のない男だな。作戦が終わっての帰り道で、あんな獲物に出会うなどとは",
    "series": "0079",
    "episode": "01",
    "person": "夏亚·阿兹纳布尔",
    "person_jp": "シャア・アズナブール"
  },
...
```

## ToDoList
- [ ] Z高达数据搜集整理 (进行中)
- [ ] 夏亚的逆袭（0093）数据搜集整理
- [ ] 0079 其他角色台词整理

## 相关应用
**微信小程序：** 夏亚每日一言 (可直接扫码进入)

![](./img/gundam-line-weapp.jpg)

## 公众号
**微信个人公众号：** 此方的手账（可扫码进入）

目前已“夏亚名台词”系列为主，每周三更新。不定期更新模型测评以及技术文章。

![](./img/qrcode.jpg)

## License
[MIT](./LICENSE)许可证
