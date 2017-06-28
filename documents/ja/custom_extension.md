# ユーザー拡張機能

## ユーザー定義定数
ユーザー定義定数は、計算式の中で自由に使える定数を定義することができる機能です。CalcNoteではデフォルトで `π` という定数が定義されており、値は `3.14159265358979323846`です。これと同様によく使う値に名前をつけて定数として定義しておけば、計算式の中でその値を定数の名前で参照することができます。

### ユーザー定義定数の一覧
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_const_list.png">

定義されている`ユーザー定義定数`の一覧が表示されます。 `+`ボタンを押すと`新規作成`、`...`ボタンを押すとメニューが表示され既存の`ユーザー定義定数`の`編集`、`削除`が可能です。

### ユーザー定義定数の編集
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_const_edit.png">

#### 定数名
定数の名前を設定します。関数名と同じ名前や、既に定義されている定数名は使用できません。また定数名の先頭の文字は数字以外である必要があります。
#### 値
定数の値を数値で設定します。設定できるのは数値のみで`%`や関数などを設定することはできません。
#### 保存ボタン
保存した`ユーザー定義定数`は計算式の中で使用することができます。定数の値を変更した場合は、既存のノートの全てに影響を及ぼします。また`キーパッドのカスタマイズ`で作成した`ユーザー定義定数`をボタンに割り当てることも可能です。

## ユーザー定義アクション
ユーザー定義アクションは、オリジナルのボタンを定義することができる機能です。例えば` + 8%`という数式を`税込`というアクション名で定義すれば、消費税を1タップで計算できるボタンが作成できます。このように普段よく使う計算をアクションとして定義しておけば、入力の手間を大幅に軽減することができます。

### ユーザー定義アクションの一覧
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_action_list.png">

定義されている`ユーザー定義アクション`の一覧が表示されます。 `+`ボタンを押すと`新規作成`、`...`ボタンを押すとメニューが表示され既存の`ユーザー定義アクション`の`編集`、`削除`が可能です。

### ユーザー定義アクションの編集
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_action_edit.png">



## ユーザー定義関数
ユーザー定義関数は、`Excel`のマクロのような機能で、オリジナルの関数を定義することができる機能です。関数は`Javascript`を使って書くことができます。条件分岐や繰り返し処理を使って複雑なビジネスロジックを実装することも可能な強力な機能ですが、作成にはプログラミングのスキルを必要とします。

### ユーザー定義関数の一覧
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_fuction_list.png">

定義されている`ユーザー定義関数`の一覧が表示されます。 `+`ボタンを押すと`新規作成`、`...`ボタンを押すとメニューが表示され既存の`ユーザー定義関数`の`編集`、`削除`が可能です。

### ユーザー定義関数の編集(定義)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_fuction_edit1.png">

### ユーザー定義関数の編集(引数)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_fuction_edit2.png">

### ユーザー定義関数の編集(コード)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_fuction_edit3.png">

### ユーザー定義関数の編集(テスト)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_fuction_edit4.png">


### 関数内で使用できるビルトイン関数
|関数|説明|
|:-----------|:------------|
val(x)|
vals(x, y)|
isRef(x)|
get(x)|
sin(x)|
asin(x)|
sinh(x)|
cos(x)|
acos(x)|
cosh(x)|
tan(x)|
atan(x)|
tanh(x)|
ln(x)|
log2(x)|
log(x)|
sqrt(x)|
cbrt(x)|
floor(x)|
ceil(x)|
round(x)|
pow(x, y)|
exp(x)|
rup(x, y)|
rdown(x, y)|
rhup(x, y)|
abs(x)|


### サンプルコード
##### 1. BMIの計算
```javascript
function bmi(height, weight) {
    var height_meter = val(height) / 100;
    return val(weight) / (height_meter * height_meter);
}
```

##### 2. ビットコインを円に変換
```javascript
function btc_jpy(btc) {
    var response = get('http://api.coindesk.com/v1/bpi/currentprice/JPY.json');
    var rate = JSON.parse(response);
    return rate.bpi.JPY.rate_float * val(btc);
}
```

<br><br>
[HOME](index.md)　[基本操作](how2use.md)　[文法](http://burton999dev.github.io/CalcNoteHelp/grammar_ja.html)　[演算子と関数](operator_and_function.md)　[単位変換](unit_converter.md)　[通貨変換](currency_converter.md)　[フローティングウィジェット](floating_widget.md)　[設定](settings.md)　[キーパッドのカスタマイズ](customizing_keypad.md)　[カスタマイズの例](example4theme.md)　[GoogleDriveプラグイン](google_drive_plugin.md)　[FAQ](faq.md)　[使用例](http://android.ascii.jp/2016/02/29/893463)  
