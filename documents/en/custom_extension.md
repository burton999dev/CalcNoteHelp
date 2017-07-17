# Custom Extension

## User Defined Constant
User defined constants allows you to define your own constants. CalcNote has constant `π` that value is `3.14159265358979323846` by the default. As well as this, you can define your constant that is a commonly used value.

### List of user defined constants
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_const_list.png">

定義されている`ユーザー定義定数`の一覧が表示されます。 `+`ボタンを押すと`新規作成`、`...`ボタンを押すとメニューが表示され既存の`ユーザー定義定数`の`編集`、`削除`が可能です。

### Editing a user defined constant
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_const_edit.png">

#### Constant Name
定数の名前を設定します。既に定義されている関数名や定数名と同じ名前は使用できません。定数名の先頭の文字は数字以外である必要があり、`_`(underscore)以外の記号は使用できません。
#### Constant Value
定数の値を数値で設定します。設定できるのは数値のみで`%`や関数などを設定することはできません。
#### Save button
保存した`ユーザー定義定数`は計算式の中で使用することができます。定数の値を変更した場合は、既存のノートの全てに影響を及ぼします。作成した`ユーザー定義定数`は`キーパッドのカスタマイズ`の設定でボタンに割り当てることができます。

## User Defined Action
ユーザー定義アクションは、オリジナルのボタンを定義することができる機能です。例えば` + 8%`という数式を`税込`というアクション名で定義すれば、消費税を1タップで計算できるボタンが作成できます。このように普段よく使う計算をアクションとして定義しておけば、入力の手間を大幅に軽減することができます。

### List of user defined actions
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_action_list.png">

定義されている`ユーザー定義アクション`の一覧が表示されます。 `+`ボタンを押すと`新規作成`、`...`ボタンを押すとメニューが表示され既存の`ユーザー定義アクション`の`編集`、`削除`が可能です。

### Editing a user defined action
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_action_edit.png">

#### Action Name
アクションの名前を設定します。アクション名はボタンに表示されます。
#### Action Value
アクションを実行した時に入力される式を設定します。値には数値や計算式、コメントなど特に制限なく設定することができます。
#### Save button
保存した`ユーザー定義アクション`は`キーパッドのカスタマイズ`の設定でボタンに割り当てるこができます。

## User Defined Function
ユーザー定義関数は、`Excel`のマクロのような機能で、オリジナルの関数を定義することができる機能です。関数は`Javascript`を使って書くことができます。条件分岐や繰り返し処理を使って複雑なビジネスロジックを実装することも可能な強力な機能ですが、作成にはプログラミングのスキルを必要とします。

### List of user defined functions
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_fuction_list.png">

定義されている`ユーザー定義関数`の一覧が表示されます。 `+`ボタンを押すと`新規作成`、`...`ボタンを押すとメニューが表示され既存の`ユーザー定義関数`の`編集`、`削除`が可能です。

### Editing a user defined function(Definition)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_fuction_edit1.png">

#### Function Name
関数の名前を設定します。既に定義されている関数名や定数名と同じ名前は使用できません。関数名に使用できる文字は英数字と`_`(underscore)のみで先頭は数字以外である必要があります。
#### Description of Function
関数の説明を設定します。説明文は関数のヘルプで表示されます。この項目は省略可能です。
#### Number of Parameters
関数の引数の数を設定します。引数の数は0個〜4個までサポートしています。
#### Description of Return Value
関数の戻り値の説明を設定します。説明文は関数のヘルプで表示されます。この項目は省略可能です。
#### NEXT button
次の画面に遷移します。

### Editing a user defined function(Parameters)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_fuction_edit2.png">

#### Parameter Name
引数の名前を設定します。デフォルトでは引数の数に応じて`p1`, `p2`, `p3`, `p4`と連番の名前が設定されます。引数名に使用できる文字は英数字と`_`(underscore)のみで先頭は数字以外である必要があります。
#### Description of Parameter
引数の説明を設定します。説明文は関数のヘルプで表示されます。この項目は省略可能です。
#### NEXT button
次の画面に遷移します。
#### BACK button
Back to the previous screen.

### Editing a user defined function(Code)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_fuction_edit3.png">

#### Source Code
`Javascript`で関数の処理を実装します。前画面で設定した関数名や引数の数など情報によって関数の定義文は自動生成されます。
#### NEXT button
次の画面に遷移します。
#### BACK button
Back to the previous screen.

### Editing a user defined function(Test)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_fuction_edit4.png">

#### Value of Argument
関数の動作確認のために引数の値を設定します。
#### ▲ Execution button
設定された引数を使って関数を呼び出します。結果が画面下部に表示されるので期待した結果か確認します。問題なければCOMPLETEボタンを押して関数を保存します。
#### COMPLETE button
関数を保存して関数一覧画面に戻ります。
#### BACK button
Back to the previous screen.

### Builtin functions for user defined functions
You can use following functions in your code.

|Function|Description|
|:-----------|:------------|
val(x)|Gets the value of parameter. You must use this function if you want to support the line reference `$n` as parameter.
vals(x, y)|Gets an array object that contains results of specified range. For instance, `vals($1, $4)` returns the results from the first line to the fourth line as an array. Returned results is array of string. so you need to call `parseInt` function.
isRef(x)|Returns a Boolean value indicating whether `x` is a line reference.
get(url)|Downloads a specified URL and returns contents of response as a string. This function is executed synchronously. The response is cached for one hour.
sin(x)|This is a built-in function of the CalcNote.
asin(x)|This is a built-in function of the CalcNote.
sinh(x)|This is a built-in function of the CalcNote.
cos(x)|This is a built-in function of the CalcNote.
acos(x)|This is a built-in function of the CalcNote.
cosh(x)|This is a built-in function of the CalcNote.
tan(x)|This is a built-in function of the CalcNote.
atan(x)|This is a built-in function of the CalcNote.
tanh(x)|This is a built-in function of the CalcNote.
ln(x)|This is a built-in function of the CalcNote.
log2(x)|This is a built-in function of the CalcNote.
log(x)|This is a built-in function of the CalcNote.
sqrt(x)|This is a built-in function of the CalcNote.
cbrt(x)|This is a built-in function of the CalcNote.
floor(x)|This is a built-in function of the CalcNote.
ceil(x)|This is a built-in function of the CalcNote.
round(x)|This is a built-in function of the CalcNote.
pow(x, y)|This is a built-in function of the CalcNote.
exp(x)|This is a built-in function of the CalcNote.
rup(x, y)|This is a built-in function of the CalcNote.
rdown(x, y)|This is a built-in function of the CalcNote.
rhup(x, y)|This is a built-in function of the CalcNote.
abs(x)|This is a built-in function of the CalcNote.

### Limitations
1. CalcNote uses [Rhino v1.7.7.1](https://github.com/mozilla/rhino) to execute Javascript.So supported feature depends on the Rhino.
2. User defined functions are compiled each time and then executed. So multiple calls to user-defined functions and complicated function can be affect performance.
3. `get` function sends a http request synchronously.

### Sample code
##### 1. Calculate the body mass index
```javascript
function bmi(height, weight) {
    var height_meter = val(height) / 100;
    return val(weight) / (height_meter * height_meter);
}
```

##### 2. Calculate the product
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

##### 3. Convert bitcoin to JPY
```javascript
function btc_jpy(btc) {
    var response = get('http://api.coindesk.com/v1/bpi/currentprice/JPY.json');
    var rate = JSON.parse(response);
    return rate.bpi.JPY.rate_float * val(btc);
}
```

<br><br>
[HOME](index.md)　[How to use](how2use.md)　[Grammar](http://burton999dev.github.io/CalcNoteHelp/grammar_en.html)　[Operators and Functions](operator_and_function.md)　[Unit Converter](unit_converter.md)　[Currency Converter](currency_converter.md)　[Floating Widget](floating_widget.md)　[Settings](settings.md)　[Customizing Keypad](customizing_keypad.md)　[CalcNotePlugin for GoogleDrive](google_drive_plugin.md)　[FAQ](faq.md)　[Customization Example](example4theme.md)  
