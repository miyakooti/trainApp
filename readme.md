## 課題
通勤通学などで駅に着くと、電車が行ったばかりで１０分程度待たされるということがしばしばある。
駅名を入力して乗換案内アプリやgoogle検索を実行すれば時間が表示されるが、いちいち打つのが面倒くさい。

## 既存の代替手段
乗換案内
google検索

## 代替手段のデメリット
電車の出発時刻を調べるタイミングは、その駅まで行くまでの歩行中ということが多い。
歩行中に文字を入力する必要があるので、歩きスマホの危険性もある。

## ターゲット
電車の移動でいそがしい大学生、社会人。特に朝とかやばい。走ってるのでググる暇もない。

## ストーリーボード
やば、電車ギリギリだな

googleで「しぶやえき、から、よこはまえき、と」

くっそーめんどくさいな、、

ん、なんか良いアプリがあるぞ。「いつくる」か、使ってみようかな。

お、すごい。文字入力をする必要がないから、ぱっと見れて便利だ！

## 実装したい機能
- よく使う駅を登録できる
- 位置の近い順に並べる
- 「つぎの電車はn分後に出発します」の機能
- 遅延情報あったらめっちゃ嬉しい。
- 登録した駅情報を、引き継ぎコードみたいなやつ発行して引き継ぐ機能
- ボタンを押したら次くる電車の情報に切り替わる機能（３つくらい表示するとかでもいいかも？わからん）
- 


## 実装
駅すぱあとapiを利用
apiを利用すると駅すぱあとfor portalのURLが手に入る

## めも
- XMLelementという形で帰ってくるらしい。swift標準のやつ
- 代替手段のデメリットを考えると、独自性のヒントとなる。
- １つのセルのデータは、出発駅名、出発駅コード(なくてもいい)、到着駅名、到着駅コード(なくてもいい)、座標、
- あと何分、とかの詳細を表示するのは、一番近い駅だけでOK？
- ニューモーフィズムやってみよう
