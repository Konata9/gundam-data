# Gundam actor lines database(gundam-lines-database)

[![license](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/0079-104-blue.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/Z-preparing-green.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/0093-preparing-green.svg?style=flat-square)]()

## Aim
This database is a byproduct when I writing the "Shyaa famous lines"(On Wechat personal offical account) series. Now have colleced 104 lines from the first gundam series (Gundam 0079). Data include japanese original line, chinese translation, speek character and episode. Japanese line all come from internet.

**PS：** I translate japanese lines to chinese myself, so if you find any wrong place please contact me by issue。

When I collecting the data, I found that there is no place put these data together. So after I collected some, I have an idea to open this database and do some convenience to Gundam's fans. You can use this data to do any good things or we can make it together.

## Data structure
Data is in JSON and SQL. The key or column are same. Files was exported by Navicat, so it can also be imported into Navicat.

**Filename rule**

gundam_lines_SeriesName_CharacterName（Alphabet）.json/sql

**key/column meaning**

No | key/colume | meaning
---- | ----- | ---- 
1 | id | MySQL key id 
2 | order | sentense order
3 | line | line chinese version
4 | line_jp | line japanese original version
5 | series | gundam series
6 | episode | episode
7 | person | speek character name in chinese
8 | person_jp | speek character name in japanese

**JSON data sample**
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
- [ ] Collect lines in Gundam Z (doing)
- [ ] Collect lines in Gundam 0093
- [ ] Collect lines in Gundam 0079 from other character

## App
**Wechat small program：** 夏亚每日一言

![](./img/gundam-line-weapp.jpg)

## Personal Offical account
**Wechat personal offical account：** 此方的手账（可扫码进入）

![](./img/qrcode.jpg)

## License
[MIT](./LICENSE)License
