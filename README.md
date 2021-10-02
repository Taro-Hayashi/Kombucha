# Kombucha トラックボールパッド
- [キット内容](#キット内容)
- [組み立て方（はんだ付け）](#組み立て方はんだ付け)
- [動作テスト](#動作テスト)
- [組み立て方（後半）](#組み立て方後半)
- [カスタマイズ](#キーマップの確認変更方法)
- [おまけ](#おまけ)

## キット内容
![パーツ一覧](img/parts.jpg)  
||部品名|数| |
|-|-|-|-|
|1|メインボード|1|黒・PCB|
|2|ミドルプレート1|1|透明・アクリル|
|3|ミドルプレート2|1|透明・アクリル|
|4|ボトムプレート|1|黒・PCB|
|5|保護プレート|1|透明・アクリル|
|6|ネジ（短）|2|3mm|
|7|ネジ（中）|7|4mm|
|8|ネジ（長）|9|6mm|
|9|スペーサー（短）|9|3mm|
|10|スペーサー（長）|7|6mm|
|11|ダイオード|12|1N4148|
|12|リセットスイッチ|1||
|13|ロータリーエンコーダ|1|EVQWGD001|
|14|ゴム足|5||

## キット以外に必要なもの
|部品名|数|||
|-|-|-|-|
|Pro Micro コンスルー付き|1||[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/promicro-spring-pinheader)|
|キースイッチ|11|Kailhロープロファイル（V1, V2)||
|キーキャップ|11|対応するもの|1U|
|7mmオプティカルトラックボールモジュール１uタイプ||[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/adtb7m)|
|トラックボールモジュール用レベル変換基板||[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/a0800tl-01-1)|
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
|フラックス||
|ピンセット||
|細いドライバー|+の1番ドライバー。|
|ニッパー等ダイオードの足を切れるもの||
|Microsoft Edge、もしくはGoogle Chrome||

## あると便利な工具
|工具名||
|-|-|
|耐熱シリコンマット||
|斜めに切ったタイプのこて先||
|温度調節可能なはんだごて|300度-350度前後。|
|テスター||
|フラックスリムーバー||
|マスキングテープ||
|はんだ吸い取り線||
|耐熱絶縁テープ（カプトンテープ）||

## 組み立て方（はんだ付け）
はんだ付けのやり方は動画で見るとわかりやすいです。  
パーツは思ったより壊れないので落ち着いて作業すると失敗しにくいです。  
 - ホームセンターのDCMさんの解説動画(58秒～)  [YouTube](https://www.youtube.com/watch?v=JFQg_ObITYE&t=58s)
  
それではダイオードをD1からD13まで取り付けます。  
足を曲げて裏から差し込みます。  
ダイオードには向きがあります。三角形の先の棒と黒線を合わせましょう。  
![](img/diode1.jpg)  
  
表で更に足を曲げて抜けないようにします。  
ダイオードと並行に曲げるとあとでキースイッチに干渉しにくいです。
![](img/diode2.jpg)  
  
はんだ付けをして足を切ります。  
![](img/diode3.jpg)  
  
はんだ付け難易度の高いレバースイッチを取り付けます。  
ランドにフラックスを塗って位置決め用の穴に合わせて乗せます。  
![](img/lever1.jpg)  
  
ピンセットでレバースイッチを押さえながら、はんだごてに乗せたはんだを手前のランドにのせていきます。  
![](img/lever2.jpg)  
  
ちょっとプラスチックを溶かしてしまいましたがこの後ちゃんと動きました。  
![](img/lever3.jpg)  
  
左右はレバーを押さえながらはんだ付けします。  
![](img/lever4.jpg)  
これら4つは取り付け強度を上げるためのランドで、電気的にはどことも繋がっていません。  
  
![](img/lever5.jpg)  
左右にある二股に分かれている接点ははんだが乗りにくいので無理に接着しなくても大丈夫です。  
  
リセットスイッチを裏から差し込み表ではんだ付けします。  
![](img/reset1.jpg)   
フラックスクリーナーを使う人はここで表面を綺麗にしておきましょう。  
![](img/reset2.jpg)   
  
キースイッチを表から差し込みます。  
![](img/keyswitch1.jpg)  
ここの二つのスイッチはPro Microと接触する可能性があるので、足を切ってからはんだ付けします。
![](img/keyswitch2.jpg)  
choc V1スイッチの場合、足が一か所干渉するので短くカットしてください。
![](img/keyswitch3.jpg)  
  
メインボードの裏にコンスルーを挿します。  
![](img/promicro1.jpg)   
コンスルーの窓が高くて両方とも同じ向きになるように設置します。  
挿すだけではんだ付けはしません。  
  
コンスルーにPro Microを挿します。TX0, RAW, USBの位置をシルク印刷と合わせましょう。  
カプトンテープをお持ちの方はここでメインボードとPro Microを絶縁しておくと安心です。  
![](img/promicro2.jpg)   
  
Pro Micro側のコンスルーの足を半田付けします。  
![](img/promicro3.jpg)   
  
SW12、SW14に表からホイール型のロータリーエンコーダーを取り付けます。  
ピンの位置を確認してツメを穴に差し込みます。  
![](img/wheel1.jpg)  
  
ツメを穴に引っかけてからピンを穴に差し込みます。  
ピンを曲げてしまわないように注意してください。  
![](img/wheel2.jpg)  
  
差し込めたらはんだ付けします。  
![](img/wheel3.jpg)  
  
SW20に表から水平型のロータリーエンコーダーを取り付けて裏からはんだ付けします。  
![](img/rot1.jpg)  
ピンが曲がらないように気を付けましょう。  
![](img/rot2.jpg)  
クリップの部分ははんだ付けしなくても構いません。  
![](img/rot3.jpg)  
  
## 動作テスト
Pro Microに動作ソフト（ファームウェア）を書き込んで動作確認をしましょう。  
キットとPCをUSBケーブルでつないでください。   

ファームウェアをダウンロードしてPro Micro Web Updaterにアクセスしてください。
- テスト用ファームウェア [handyman_test.hex](https://github.com/Taro-Hayashi/Handyman/releases/download/14.6/handyman_test.hex)
- Pro Micro Web Updater https://sekigon-gonnoc.github.io/promicro-web-updater/index.html

ファイルの選択ボタンを押してダウンロードしたファームウェアを指定したら、flashボタンを押しましょう。  
![](img/promicrowebupdater1.jpg)  

ブラウザのアドレスバーからメッセージが出てきたら、キットのリセットスイッチを押します。      
すると選択欄にArduino Microが出てきてクリックできるようになります。  
![](img/promicrowebupdater2.jpg)  

選択して接続を押すと書き込みが終わります。  
![](img/promicrowebupdater3.jpg)  
ファームウェアを更新する時もこの手順で行います。  

アドレスバーやテキストエディタを使ってすべてのスイッチが反応することを確かめてください。
お疲れ様でした。問題がなければはんだ付けは終了です。

## 組み立て方（後半）
USBケーブルを抜いてプレートを組付けます。  
アクリルからは保護フィルムを剥がしてください。割れやすいので気をつけましょう。  

![](img/bottom1.jpg)  
メインボードの赤丸のネジ穴にスペーサー（中）とスペーサー（短）を止めます。  
画像のようにスイッチがついてる側にスペーサー（中）があるようにしてください。  
![](img/bottom2.jpg)  
  
メインボード裏面の残りのネジ穴にスペーサー（短）をネジ（短）で取り付けてミドルプレート1（透明）を嵌めます。
![](img/bottom3.jpg)  

ミドルプレート2とバックプレートをネジ（長）で止めます。
![](img/bottom4.jpg)  
![](img/bottom5.jpg)  

表に保護プレートをネジ（中）で取り付けましょう。
![](img/bottom6.jpg)  

キーキャップを取り付けたら本番用のファームウェアに更新しましょう。
- [handyman_via.hex](https://github.com/Taro-Hayashi/Handyman/releases/download/14.6/handyman_via.hex)

マイナスドライバーでノブを取りつけ、ゴム足を貼ったら完成です。
![](img/nob.jpg)  
ノブは直径20mmのものまで取り付けを確認しました。  
![](img/full.jpg)  

## キーマップの確認、変更方法
標準ではUS配列設定でのClip Studio Paintにあわせたキーマップになっています。  
![](img/layout.png)  
[Keyboard Layout Editor で見る](http://www.keyboard-layout-editor.com/#/gists/b1de3d8b33b46ababd2dff071c8af257)  

使わないキーを削除したり使用頻度の高いキーを押しやすい位置に変更してみましょう。  
  
ChromeかEdgeでRemapにアクセスしてください。  
- Remap https://remap-keys.app/
  
![](img/remap1.png)  
左を選んで進んでいくとアドレスバーからメッセージが出てキーボードを選択できます。  
  
ドラッグアンドドロップで変更が終わったら右上のflashボタンを押すと反映されます。  
![](img/remap3.png)  
  
## その他
ファームウェアのフォルダ  
https://github.com/Taro-Hayashi/qmk_firmware/tree/master/keyboards/kombucha
  
VIA用JSONファイル [kombucha.json](https://github.com/Taro-Hayashi/Handyman/releases/download/1.0/kombucha.json)  
  
プレートのデザインデータ  
[handyman_plates.zip](https://github.com/Taro-Hayashi/Handyman/releases/download/1.0/kombucha_plates.zip)  
発注先のルールに沿ってデータを修正してください。  
  
ご不明な点があればBOOTHのメッセージかtwitterでいつでも聞いてください。  
BOOTH: https://tarohayashi.booth.pm/items/3208122  
  
foostan様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/foostan/kbd/  
https://github.com/foostan/kbd/blob/master/LICENSE  
  
plut0nium様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/plut0nium/0xLib  
https://github.com/plut0nium/0xLib/blob/master/LICENSE.txt  
  
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />この キット は <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">クリエイティブ・コモンズ 表示 - 継承 4.0 国際 ライセンス</a>の下に提供されています。
