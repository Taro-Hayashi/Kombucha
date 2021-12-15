# Kombucha トラックボール
- [キット内容](#キット内容)
- [組み立て方（はんだ付け）](#組み立て方はんだ付け)
- [動作テスト](#動作テスト)
- [組み立て方（後半）](#組み立て方後半)
- [カスタマイズ](#キーマップの確認変更方法)
- [おまけ](#おまけ)

## キット内容
![パーツ一覧](img/IMG_2550.jpg)  
||部品名|数| |
|-|-|-|-|
|1|メインボード|1|黒・PCB|
|2|ボトムプレート|1|黒・PCB|
|3|ミドルプレート1|1|透明・アクリル|
|4|ミドルプレート2|1|透明・アクリル|
|5|保護プレート|1|透明・アクリル|
|6|ネジ（短）|2|3mm|
|7|ネジ（中）|7|4mm|
|8|ネジ（長）|9|6mm|
|9|スペーサー（短）|9|3mm|
|10|スペーサー（長）|7|6mm|
|11|ダイオード|12|1N4148|
|12|リセットスイッチ|1||
|13|ロータリーエンコーダ|1|EVQWGD001|
|14|ゴム足|4||

## キット以外に必要なもの
|部品名|数|||
|-|-|-|-|
|Pro Micro コンスルー付き|1||[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/promicro-spring-pinheader)|
|キースイッチ|11|Kailhロープロファイル（V1, V2)||
|キーキャップ|11|対応するもの||
|7mmオプティカルトラックボールモジュール１uタイプ|1||[遊舎工房様](https://shop.yushakobo.jp/products/adtb7m)、[ビットトレードワン様](https://btoshop.jp/products/adtb7m)、[Amazon](https://www.amazon.co.jp/dp/B087BVNWYS)|
|トラックボールモジュール用レベル変換基板|1||[遊舎工房様](https://shop.yushakobo.jp/products/a0800tl-01-1)、[のぎけす屋様](https://booth.pm/ja/items/2008258)|
|OLED用ピンヘッダ|1||[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/a1600ph-01-1)|
|OLED用ピンソケット|1||[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/a1600ps-01-1)|
|Micro USB ケーブル|1||
  
## オプション
|部品名|数|||
|-|-|-|-|
|SK6812MINI-E|11|[取り付け方](led.md)|[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/sk6812mini-e-10)|
|WS2812B|6|無くてもバックライトだけ光ります。|[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/a0800ws-01-10)|
|1N4148W|12|表面実装タイプのダイオード|[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/a0800di-02-100)|
 
## 必要な工具
|工具名| |
|-|-|
|はんだごて||
|はんだごて置き場||
|鉛入りはんだ||
|細いドライバー|+の1番ドライバー。|
|ニッパー等ダイオードの足を切れるもの||
|Microsoft Edge、もしくはGoogle Chrome||

## あると便利な工具
|工具名||
|-|-|
|耐熱シリコンマット||
|斜めに切ったタイプのこて先||
|温度調節可能なはんだごて|300度-350度前後。|
|フラックス|LEDを付けるのなら|
|ピンセット|LEDを付けるのなら|
|テスター||
|フラックスリムーバー||
|マスキングテープ||
|はんだ吸い取り線||
|耐熱絶縁テープ（カプトンテープ）||

## 組み立て方（はんだ付け）
はんだ付けのやり方は動画で見るとわかりやすいです。  
パーツは思ったより壊れないので落ち着いて作業すると失敗しにくいです。  
 - ホームセンターのDCMさんの解説動画(58秒～)  [YouTube](https://www.youtube.com/watch?v=JFQg_ObITYE&t=58s)
  
それではダイオードをD1からD12まで取り付けます。  
足を曲げて裏から差し込みます。  
ダイオードには向きがあります。三角形の先の棒と黒線を合わせましょう。  
![](img/diode1.jpg)  
  
表で更に足を曲げて抜けないようにします。  
ダイオードと並行に曲げるとあとでキースイッチに干渉しにくいです。
![](img/diode2.jpg)  
  
はんだ付けをして足を切ります。  
![](img/diode3.jpg)  

裏からTB1にOLED用ピンソケットを差し込み、表ではんだ付けします。  
![](img/socket1.jpg)  
気軽に交換ができなくなりますが、ピンソケットなしではんだ付けしてしまっても構いません。
フラックスクリーナーを使う場合はここで表面を綺麗にしましょう。  
![](img/socket2.jpg)  

リセットスイッチを表から差し込み裏ではんだ付けします。  
![](img/reset.jpg)   
  
キースイッチを表から差し込みはんだ付けします。  
![](img/keyswitch1.jpg)  
ここの二つのスイッチはPro Microと接触する可能性があるので、足を切ってからはんだ付けします。
![](img/keyswitch2.jpg)  
  
メインボードの裏にコンスルーを挿します。  
![](img/promicro1.jpg)  
※新品のPro Microが無かったので別のキットの写真ですが、同様に作っていただいて大丈夫です。  
コンスルーの窓が高くて両方とも同じ向きになるように設置します。  
挿すだけではんだ付けはしません。  
  
コンスルーにPro Microを挿します。TX0, RAW, USBの位置をシルク印刷と合わせましょう。  
カプトンテープをお持ちの方はここでメインボードとPro Microを絶縁しておくと安心です。  
![](img/promicro2.jpg)   
※新品のPro Microが無かったので別のキットの写真ですが、同様に作っていただいて大丈夫です。
  
Pro Micro側のコンスルーの足を半田付けします。  
![](img/promicro3.jpg)   
Pro Microを設置する場所は表側と裏側に2か所あります。 
使いやすい方を使ってください。  
  
SW6に表からホイール型のロータリーエンコーダーを取り付けます。  
ピンの位置を確認してツメを穴に差し込みます。  
![](img/wheel1.jpg)  
  
ツメを穴に引っかけてからピンを穴に差し込みます。  
ピンを曲げてしまわないように注意してください。  
![](img/wheel2.jpg)  
  
差し込めたらはんだ付けします。  
![](img/wheel3.jpg)  
  
トラックボール、レベル変換基板、OLED用ピンヘッダを画像のようにはんだ付けしましょう。  
![](img/track1.jpg)  

表からレベル変換基板を通します。  
![](img/track2.jpg)  

裏面のピンソケットにピンヘッダを差し込みます。  
![](img/track3.jpg)  
  
## 動作テスト
Pro Microに動作ソフト（ファームウェア）を書き込んで動作確認をしましょう。  
キットとPCをUSBケーブルでつないでください。   

下のwebサイトにアクセスしてください。
- https://remap-keys.app/catalog/08BHJ3OcLCe716TwOdDz/firmware

テストファームウェアを選んでFLASHします。
![](img/remap02.jpg)  
![](img/remap03.jpg)  

キットのリセットスイッチを押すとArduino Microが現れるので、クリックして接続します。
![](img/remap04.jpg) 

書き込みが完了したらウィンドウを閉じて大丈夫です。
![](img/remap05.jpg) 

アドレスバーやテキストエディタを使ってすべてのスイッチが反応することを確かめてください。  
お疲れ様でした。問題がなければはんだ付けは終了です。

## 組み立て方（後半）
USBケーブルを抜いてプレートを組付けます。  
アクリルからは保護フィルムを剥がしてください。割れやすいので気をつけましょう。  

メインボードの赤丸のネジ穴にスペーサー（長）とスペーサー（短）を止めます。 
![](img/bottom1.jpg)   
画像のようにスイッチがついてる側にスペーサー（短）があるようにしてください。  
![](img/bottom2.jpg)  

トラックボールが円形の穴に綺麗に収まるように保護プレートをネジ（中）で止めます。
![](img/bottom3.jpg)  
  
メインボードの残りのネジ穴にスペーサー（短）をネジ（短）で取り付けてミドルプレート1（透明）を嵌めます。
![](img/bottom4.jpg)  
トラックボールのケーブルを間に挟んでしまわないように気を付けてください。

ミドルプレート2とバックプレートをネジ（長）で止めます。
![](img/bottom5.jpg)  

![](img/bottom6.jpg)  

キーキャップを取り付けたら先ほどと同様の手順で本番用のファームウェアに更新しましょう。
- https://remap-keys.app/catalog/08BHJ3OcLCe716TwOdDz/firmware
![](img/remap06.jpg)  

裏面4隅にゴム足を貼ったら完成です。  
![](img/full.jpg)  

## キーマップの確認、変更方法
![](img/keymap.jpg)  
[Keyboard Layout Editor で見る](http://www.keyboard-layout-editor.com/#/gists/8a9cd944cc1cf5abed875719608a3e3a)  

使わないキーを削除したり使用頻度の高いキーを押しやすい位置に変更してみましょう。  
  
ChromeかEdgeでRemapにアクセスしてください。  
- Remap https://remap-keys.app/
  
![](img/remap1.png)  
左を選ぶとキーボードを選択できます。  
![](img/remap2.)  
ドラッグアンドドロップで変更が終わったら右上のflashボタンを押すと反映されます。  
![](img/remap3.png)  
  
## その他

ファームウェアのフォルダ  
https://github.com/Taro-Hayashi/qmk_firmware/tree/master/keyboards/kombucha
  
VIA用JSONファイル [kombucha.json](https://github.com/Taro-Hayashi/Kombucha/releases/download/14.15/kombucha.json)  
  
プレートのデザインデータ  
[kombucha_plates.zip](https://github.com/Taro-Hayashi/Kombucha/releases/download/14.31/kombucha_plates.zip)  
発注先のルールに沿ってデータを修正してください。  
  
ご不明な点があればBOOTHのメッセージかtwitterでいつでも聞いてください。  
  
foostan様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/foostan/kbd/  
https://github.com/foostan/kbd/blob/master/LICENSE  
  
plut0nium様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/plut0nium/0xLib  
https://github.com/plut0nium/0xLib/blob/master/LICENSE.txt  
  
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />この キット は <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">クリエイティブ・コモンズ 表示 - 継承 4.0 国際 ライセンス</a>の下に提供されています。

- BOOTH: https://tarohayashi.booth.pm/items/3252673  
