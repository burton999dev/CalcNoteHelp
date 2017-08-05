# 通貨変換
`CalcNote`は通貨変換をサポートしています。サポートしている通貨は `USD`, `EUR`, `JPY`, `GBP`, `CHF`, `AUD`, `CAD`, `CNY`, `RUB`, `NZD`, `HKD`, `KRW`, `BGN`, `BRL`, `INR`, `CZK`, `DKK`, `HRK`, `HUF`, `IDR`, `ILS`, `MXN`, `MYR`, `NOK`, `PHP`, `PLN`, `RON`, `SEK`, `SGD`, `THB`, `TRY` 31通貨です。通貨変換は専用の入力パッドを使って直接値を入力するか、`通貨変換関数`として入力することもできます。為替レートは1日1回の頻度で更新されます。リアルタイムな正確なレートではないので注意してください。

## 通貨変換用の入力パッド
通貨変換用の入力パッドは[キーパッドのカスタマイズ](customizing_keypad.md)の設定から、表示をONにすることで使用できます。変換元の値と変換元の通貨を入力すると変換後の通貨がリスト表示されます。リストの <img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_paste_value_black_24dp.png" width="20px" align="top"> を押すと変換後の値が入力され、 <img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_paste_function_black_24dp.png" width="20px" align="top"> を押すと変換元の値を引数とした関数として入力されます。
<br/>
<br/>
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/currency_converter.png">

### 通貨一覧
|通貨コード|関数で使用する通貨名|説明|
|:-----------|:------------|:------------|
USD|usd|米ドル
EUR|eur|ユーロ
JPY|jpy|日本円
GBP|gbp|英ポンド
CHF|chf|スイスフラン
AUD|aud|豪ドル
CAD|cad|カナダドル
CNY|cny|人民元
RUB|rub|ロシアルーブル
NZD|nzd|ニュージーランドドル
HKD|hkd|香港ドル
KRW|krw|韓国ウォン
BGN|bgn|ブルガリアレフ
BRL|brl|ブラジルレアル
INR|inr|インドルピー
CZK|czk|チェココルナ
DKK|dkk|デンマーククローネ
HRK|hrk|クロアチアクーナ
HUF|huf|ハンガリーフォリント
IDR|idr|インドネシアルピア
ILS|ils|イスラエルシュケル
MXN|mxn|メキシコペソ
MYR|myr|マレーシアリンギット
NOK|nok|ノルウェイクローネ
PHP|php|フィリピンペソ
PLN|pln|ポーランドズウォティ
RON|ron|新ルーマニアレイ
SEK|sek|スウェーデンクローナ
SGD|sgd|シンガポールドル
THB|thb|タイバーツ
TRY|try|トルコリラ

<br><br>
[HOME](index.md)　[基本操作](how2use.md)　[文法](http://burton999dev.github.io/CalcNoteHelp/grammar_ja.html)　[演算子と関数](operator_and_function.md)　[単位変換](unit_converter.md)　[フローティングウィジェット](floating_widget.md)　[設定](settings.md)　[キーパッドのカスタマイズ](customizing_keypad.md)　[カスタマイズの例](example4theme.md)　[ユーザー拡張機能](custom_extension.md)　[GoogleDriveプラグイン](google_drive_plugin.md)　[FAQ](faq.md)　[使用例](http://android.ascii.jp/2016/02/29/893463)  

