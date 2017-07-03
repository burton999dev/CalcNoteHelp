# ユーザー拡張機能

## ユーザー定義定数
ユーザー定義定数は、計算式の中で自由に使える定数を定義することができる機能です。CalcNoteではデフォルトで `π` という定数が定義されており、値は `3.14159265358979323846`です。これと同様によく使う値に名前をつけて定数として定義しておけば、計算式の中でその値を定数の名前で参照することができます。数学や物理の勉強でCalcNoteを使用している方に便利な機能です。

### ユーザー定義定数の一覧
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_const_list.png">

定義されている`ユーザー定義定数`の一覧が表示されます。 `+`ボタンを押すと`新規作成`、`...`ボタンを押すとメニューが表示され既存の`ユーザー定義定数`の`編集`、`削除`が可能です。

### ユーザー定義定数の編集
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_const_edit.png">

#### 定数名
定数の名前を設定します。既に定義されている関数名や定数名と同じ名前は使用できません。定数名の先頭の文字は数字以外である必要があり、`_`(underscore)以外の記号は使用できません。
#### 値
定数の値を数値で設定します。設定できるのは数値のみで`%`や関数などを設定することはできません。
#### 保存ボタン
保存した`ユーザー定義定数`は計算式の中で使用することができます。定数の値を変更した場合は、既存のノートの全てに影響を及ぼします。作成した`ユーザー定義定数`は`キーパッドのカスタマイズ`の設定でボタンに割り当てることができます。

## ユーザー定義アクション
ユーザー定義アクションは、オリジナルのボタンを定義することができる機能です。例えば` + 8%`という数式を`税込`というアクション名で定義すれば、消費税を1タップで計算できるボタンが作成できます。このように普段よく使う計算をアクションとして定義しておけば、入力の手間を大幅に軽減することができます。

### ユーザー定義アクションの一覧
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_action_list.png">

定義されている`ユーザー定義アクション`の一覧が表示されます。 `+`ボタンを押すと`新規作成`、`...`ボタンを押すとメニューが表示され既存の`ユーザー定義アクション`の`編集`、`削除`が可能です。

### ユーザー定義アクションの編集
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_action_edit.png">

#### アクション名
アクションの名前を設定します。アクション名はボタンに表示されます。
#### 値
アクションを実行した時に入力される式を設定します。値には数値や計算式、コメントなど特に制限なく設定することができます。
#### 保存ボタン
保存した`ユーザー定義アクション`は`キーパッドのカスタマイズ`の設定でボタンに割り当てるこができます。

## ユーザー定義関数
ユーザー定義関数は、`Excel`のマクロのような機能で、オリジナルの関数を定義することができる機能です。関数は`Javascript`を使って書くことができます。条件分岐や繰り返し処理を使って複雑なビジネスロジックを実装することも可能な強力な機能ですが、作成にはプログラミングのスキルを必要とします。

### ユーザー定義関数の一覧
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_fuction_list.png">

定義されている`ユーザー定義関数`の一覧が表示されます。 `+`ボタンを押すと`新規作成`、`...`ボタンを押すとメニューが表示され既存の`ユーザー定義関数`の`編集`、`削除`が可能です。

### ユーザー定義関数の編集(定義)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_fuction_edit1.png">

#### 関数名
関数の名前を設定します。既に定義されている関数名や定数名と同じ名前は使用できません。関数名に使用できる文字は英数字と`_`(underscore)のみで先頭は数字以外である必要があります。
#### 関数の説明
関数の説明を設定します。説明文は関数のヘルプで表示されます。この項目は省略可能です。
#### 引数の数
関数の引数の数を設定します。引数の数は0個〜4個までサポートしています。
#### 戻り値の説明
関数の戻り値の説明を設定します。説明文は関数のヘルプで表示されます。この項目は省略可能です。
#### NEXTボタン
次の画面に遷移します。

### ユーザー定義関数の編集(引数)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_fuction_edit2.png">

#### 引数の名前
引数の名前を設定します。デフォルトでは引数の数に応じて`p1`, `p2`, `p3`, `p4`と連番の名前が設定されます。引数名に使用できる文字は英数字と`_`(underscore)のみで先頭は数字以外である必要があります。
#### 引数の説明
引数の説明を設定します。説明文は関数のヘルプで表示されます。この項目は省略可能です。
#### NEXTボタン
次の画面に遷移します。
#### BACKボタン
前の画面に遷移します。

### ユーザー定義関数の編集(コード)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_fuction_edit3.png">

#### コード
`Javascript`で関数の処理を実装します。前画面で設定した関数名や引数の数など情報によって関数の定義文は自動生成されます。
#### NEXTボタン
次の画面に遷移します。
#### BACKボタン
前の画面に遷移します。

### ユーザー定義関数の編集(テスト)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/user_fuction_edit4.png">

#### 引数の値
関数の動作確認のために引数の値を設定します。
#### ▲実行ボタン
設定された引数を使って関数を呼び出します。結果が画面下部に表示されるので期待した結果か確認します。問題なければCOMPLETEボタンを押して関数を保存します。
#### COMPLETEボタン
関数を保存して関数一覧画面に戻ります。
#### BACKボタン
前の画面に遷移します。

### 関数内で使用できるビルトイン関数
ユーザー定義関数では`Javascript`の機能以外に以下の関数を使用することができます。

|関数|説明|
|:-----------|:------------|
val(x)|引数の値を取得します。引数をこの関数で処理しないと引数が行参照`$n`の場合に正常に動作しません。
vals(x, y)|2つの行参照`$n`の間の値を配列で取得します。例えば`vals($1, $4)`の場合、1行目から4行目の答えが配列で返されます。返される配列は文字列の配列なので、`parseInt`などで数値に変換する必要があります。
isRef(x)|与えられた引数が行参照`$n`の場合に`true`を返します。
get(x)|引数に指定した`URL`に`HTTP GET`してレスポンスを文字列で返します。通信は同期的に行われるので、アプリが一瞬フリーズしたようになります。レスポンスは1時間キャッシュされます。あくまで試験的な機能で利用は推奨しません。
sin(x)|CalcNoteで利用できる`sin`関数です。
asin(x)|CalcNoteで利用できる`asin`関数です。
sinh(x)|CalcNoteで利用できる`sinh`関数です。
cos(x)|CalcNoteで利用できる`cos`関数です。
acos(x)|CalcNoteで利用できる`acos`関数です。
cosh(x)|CalcNoteで利用できる`cosh`関数です。
tan(x)|CalcNoteで利用できる`tan`関数です。
atan(x)|CalcNoteで利用できる`atan`関数です。
tanh(x)|CalcNoteで利用できる`tanh`関数です。
ln(x)|CalcNoteで利用できる`ln`関数です。
log2(x)|CalcNoteで利用できる`log2`関数です。
log(x)|CalcNoteで利用できる`log`関数です。
sqrt(x)|CalcNoteで利用できる`sqrt`関数です。
cbrt(x)|CalcNoteで利用できる`cbrt`関数です。
floor(x)|CalcNoteで利用できる`floor`関数です。
ceil(x)|CalcNoteで利用できる`ceil`関数です。
round(x)|CalcNoteで利用できる`round`関数です。
pow(x, y)|CalcNoteで利用できる`pow`関数です。
exp(x)|CalcNoteで利用できる`exp`関数です。
rup(x, y)|CalcNoteで利用できる`rup`関数です。
rdown(x, y)|CalcNoteで利用できる`rdown`関数です。
rhup(x, y)|CalcNoteで利用できる`rhup`関数です。
abs(x)|CalcNoteで利用できる`abs`関数です。


### サンプルコード
##### 1. BMIの計算
```javascript
function bmi(height, weight) {
    var height_meter = val(height) / 100;
    return val(weight) / (height_meter * height_meter);
}
```

##### 2. 総乗の計算
```javascript
function product(p1, p2) {
    var values;
    if (isRef(p1) && isRef(p2)) {
        values = vals(p1, p2);
    } else {
        values = [val(p1), val(p2)];
    }
    var total = 1;
    values.forEach(function(value) {
        total *= parseInt(value);
    });
    return total;
}
```

##### 3. ビットコインを円に変換
```javascript
function btc_jpy(btc) {
    var response = get('http://api.coindesk.com/v1/bpi/currentprice/JPY.json');
    var rate = JSON.parse(response);
    return rate.bpi.JPY.rate_float * val(btc);
}
```

<br><br>
[HOME](index.md)　[基本操作](how2use.md)　[文法](http://burton999dev.github.io/CalcNoteHelp/grammar_ja.html)　[演算子と関数](operator_and_function.md)　[単位変換](unit_converter.md)　[通貨変換](currency_converter.md)　[フローティングウィジェット](floating_widget.md)　[設定](settings.md)　[キーパッドのカスタマイズ](customizing_keypad.md)　[カスタマイズの例](example4theme.md)　[GoogleDriveプラグイン](google_drive_plugin.md)　[FAQ](faq.md)　[使用例](http://android.ascii.jp/2016/02/29/893463)  
