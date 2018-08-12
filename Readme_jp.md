# ガンダムセリフデータベース(gundam-lines-database)

[![license](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/0079-104-blue.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/Z-143-blue.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/0093-39-blue.svg?style=flat-square)]()
[![0079](https://img.shields.io/badge/sp-2-blue.svg?style=flat-square)]()

## 目的
このデータベースは“シャア名言”シリーズ（WeChat個人公式アカウントで発表され、中国語でシャアのセリフを紹介する文章である）を作る時のものです。今はガンダムUC宇宙シリーズの名言を収録し、ファーストガンダム：104句、Zガンダム：143句、逆襲のシャア：39句、ほかSP：2編。内容は日本語セリフ、人物とエピソードを含めて、日本語セリフはすべてインターネット上から集めたものである。

データ集める時、ガンダムシリーズの名言は多くが、ネット中でバラバラしている。そして、データ集めた後、公開データベースにする思いが付きました。多分ガンダムファンに役に立つと思ている。このデータを利用して、何かを作るといいが、またみんなで一緒に作るといい。

## データストラクチャー
データはJSONとSQL二つタイプのファイルがあって、キーや列は同じである。全部はNavicatでエクスポートしたため、Navicatでインポートすることも可能です。

**命名ルール**

gundam_lines_シリーズ名_人物名（ローマ字）.json/sql

**列（キー）の意義**

No | 列（キー） | 意義
---- | ----- | ---- 
1 | id | MySQL 主キーのid 
2 | order | セリフ順番
3 | line_jp | セリフの日本語
4 | series | シリーズ名 
5 | episode | エピソード数
6 | person | 人物名中国語翻訳
7 | person_jp | 人物名日本語

**JSONデータサンプル**
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
- [x] ガンダムZのセリフの集め 
- [x] シャアの逆襲のセリフの集め
- [ ] ファーストガンダム他のキャラーのセリフの集め

## 関連アプリ
**WeChatアプリ：** 夏亚每日一言 (下のコードでスキャン)

![](./img/wechat-app.jpg)

## 個人公式アカウント
**WeChat個人公式アカウント：** 此方的手账（下のコードでスキャン）

![](./img/wechat-qr.jpg)

## License
[MIT](./LICENSE)ライセンス
