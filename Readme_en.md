# Gundam actor lines database(gundam-lines-database)

[![license](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/0079-104-blue.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/Z-143-blue.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/0093-39-blue.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/sp-2-blue.svg?style=flat-square)]()

## Aim
This database is a byproduct when I writing the "Shyaa famous lines"(On Wechat personal offical account) series. Now have colleced from the gundam series (Gundam 0079: 104, Gundam Z: 143, Gundam 0093: 39, SP: 2). Data include japanese original line, speek character and episode. Japanese line all come from internet.

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
3 | line_jp | line japanese original version
4 | series | gundam series
5 | episode | episode
6 | person | speek character name in chinese
7 | person_jp | speek character name in japanese

**JSON data sample**
```json
...
{
"﻿id":"1",
"order":"1",
"line_jp":"私もよくよく運のない男だな。作戦が終わっての帰り道で、あんな獲物に出会うなどとは",
"series":"0079",
"episode":"01",
"person":"夏亚·阿兹纳布尔",
"person_jp":"シャア・アズナブール"
},
...
```

## ToDoList
- [x] Collect lines in Gundam Z 
- [x] Collect lines in Gundam 0093
- [ ] Collect lines in Gundam 0079 from other character

## App
**Wechat small program：** 夏亚每日一言

![](./img/wechat-app.jpg)

## Personal Offical account
**Wechat personal offical account：** 此方的手账（可扫码进入）

![](./img/wechat-qr.jpg)

## License
[MIT](./LICENSE)License
