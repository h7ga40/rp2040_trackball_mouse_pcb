# PCB for Kensington trackball with RP2040

[Kensington Orbit Trackball with Scroll Ring](https://www.kensington.com/p/products/electronic-control-solutions/trackball-products/orbit-trackball-with-scroll-ring/)の基板を[PGA2040](https://shop.pimoroni.com/products/pga2040)を使っ基板に置き換えるためのKiCadプロジェクト

**まだホイールがぎこちないです**。本物の回路の読み取ったコンパレータ回路が原因？

![Trackball](images/appearance.jpg)

## 基板発注時の注意

板厚は**1.2mm**です。

## 主要部品

|部品|入手先|備考|
|-|-|-|
|PGA2040|<https://akizukidenshi.com/catalog/g/gM-16762/>|Raspberry pi picoと同じCPU|
|IR928-6C-F|<https://www.marutsu.co.jp/pc/i/12907560/>|ホイール用２相エンコーダのLED</br>見た目が同じなので選択|
|PT5529B/L2/H3|<https://www.marutsu.co.jp/pc/i/13719542/>|ホイール用２相エンコーダのフォトトランジスタ</br>見た目が同じなので選択|
|LMV393D|<https://www.marutsu.co.jp/pc/i/30637519/>|２相エンコーダ信号用のコンパレータ|
|B6B-PH-K-S|<https://www.marutsu.co.jp/pc/i/46628/>|ADNS-5050との接続用コネクタ|
|S5B-PH-K-S|<https://www.marutsu.co.jp/pc/i/54957/>|USBケーブルとの接続用コネクタ|
|kailh mute switch|<https://www.amazon.co.jp/s?k=kailh+mute+switch>|マウスボタン</br>[秋月のタクトスイッチ](https://akizukidenshi.com/catalog/g/gP-14892/)で代用（底上げが必要）|
|タクトスイッチ|<https://akizukidenshi.com/catalog/g/gP-06184/>|RP2040のリセットとモード選択用|

## ソフトウェア

[こちら](https://github.com/h7ga40/rp2040_trackball_mouse)にソフトウェアがあります。

## 部品実装

PGA2040周辺はこのような感じ

![PGA2040周辺](images/pga2040.jpg)

## その他の情報

[コネクテッド・マウス](https://www.slideshare.net/HiroakiNagashima1/ss-250643168)
