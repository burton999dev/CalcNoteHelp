# How to use
The `CalcNote` is a calculator but it has appearance similar to the notepad.So you might be confused but it's simple and easy to use.  
This section describes the basic usage of CalcNote.  

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/screen_description.png">

|Area|Description|
|:-----------|:------------|
LineNo|Show the line number. You can input the [Line references](#lineno) to tap the line number.<br>This area can be hidden by [Editor Settings](settings.md).
Editor Area|Write the expression to calculate your problems. You can copy, cut or paste a expression like a notepad.
Results Area|Calculation results are displayed. The results are calculated in real-time when you write a expression on the editor.<br>You can show the result as hexadecimal, binary, tax included and tax excluded to tap the result. You need to configure tax rate if you want to calculate the tax included and tax excluded.
Toatal Area|A running total of all your lines is displayed.<br>You can show the result as hexadecimal, binary, tax included and tax excluded to tap the result. You need to configure tax rate if you want to calculate the tax included and tax excluded.
Keypad|You can switch the keypad to swipe to left or right.There are three keypads.<br>[Numeric keypad] <-> [Function keypad] <-> [Hexadecimal keypad]
Keypad Switches|You can show/hide the software keyboard. And also you can show/hide the keypad.

## Menu
You can access various functions via side menu.  You can show the side menu to tap the action bar menu or to swipe from the left side to the right side or tap the hardware menu key.

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/open_menu.png">
<br>
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/menu_description.png">

|Menu Item|Description|
|:-----------|:------------|
New File|編集中の計算式を下書きとして保存して、新規ファイルを作成します。
Save|編集中の計算式を名前を付けて保存します。
Export|編集中の計算式をクリップボードにコピーしたり、他のアプリケーションに共有することができます。
Format expression|編集中の式を整形して見やすくします。
Settings|[設定画面](settings.md)に遷移します。
Online Help|Jump to this page using default browser
Drafts|下書きの一覧が表示されます。選択すると下書きを開きます。<br>ゴミ箱のアイコンをタップすると下書きを削除できます。
Saved Files|名前を付けて保存したファイルの一覧が表示されます。選択するとファイルを開きます。<br>ゴミ箱のアイコンをタップするとファイルを削除できます。

## <a name ="lineno">Line no and Line references</a>
行番号をタップするとその行の答えを参照するための変数 `${LineNo}` が入力されます。参照変数は複雑な計算を簡単な式に分割して計算する時に便利です。改行の入力によって参照している行番号が変わった場合は、参照変数も自動的に更新されます。現時点では参照できる行は前の行のみになります。例えば5行目に `$6` と書いても6行目を参照することはできません。

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/line_no.png">

## Editor Area
ここに計算式を書くことでリアルタイムで結果領域の答えが表示されます。計算式は <img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_return_black_18dp.png" width="20px" align="top"> をタップして改行することで何個でも書くことができます。結果は1行毎に別々に計算され結果領域に表示されます。計算式が長い場合は自動的に折り返して表示され複数行になることがありますが、結果は1行として扱われます。

## Results Area and Total Area
結果の数値をタップすると結果の2進数、16進数、消費税込、税別の金額が計算されポップアップで表示されます。それぞれの結果はタップすることでクリップボードにコピーされます。また行番号をタップすると編集領域に `${LineNo}` が入力されます。

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/result_popup1.png">
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/result_popup2.png">

## Keypad
**入力パッドの高さはデフォルトで、お使いの文字入力ソフトのソフトウェアキーボードの高さに合わせた高さになります。**お使いのソフトウェアキーボードがコンパクトな場合、入力パッドも小さくなり押しづらくなる可能性があります。その場合は、[設定](settings.md)で入力パッドの高さを自分で調整するか、文字入力ソフトの設定でソフトウェアキーボードの高さを調整することで改善することができます。  
入力パッドは左右にスワイプすることで、切り替えることができます。現時点では３種類の入力パッドをサポートしています。各ボタンの右下に `...` 三点リーダが表示されているボタンはロングタップすると関連するボタンがポップアップ表示されます。例えば「削除ボタン」をロングタップすると「全削除ボタン」と「1行削除ボタン」が表示されます。


<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/keypad.png">
<br>
**Popup buttons that appears by the long tap**  

|Button|Long tap 1|Long tap 2|
|:-----------|:------------|:------------|
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_backspace_black_18dp.png">|Clear all|Clear line
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_return_black_18dp.png">|`${LineNo}`|
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_arrow_left_bold_black_18dp.png">|Move to the beginning of the line|Select to the beginning of the line
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_arrow_right_bold_black_18dp.png">|Mode to the end of the line|Select to the end of the line
**×**|**()**|
**÷**|**mod**|
**.**|**,**|
**sin**|**asin**|**sinh**
**cos**|**acos**|**cosh**
**tan**|**atan**|**tanh**
**log**|**log2**|**ln**
**round**|**round half up**|
**ceil**|**round up**|
**floor**|**round down**|
**√**|**cbrt**|
**!**|**nPr**|**nCr**
**^**|**^2**|**^3**

### Keypad for parameters
When you input such as `√`, `^` or functions, popup keypad will be shown. You can input argument easily. You can input an argument easily.

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/function_pad.png">

## Keypad Switches
|Button|Description|
|:-----------|:------------|
123|Hide the software keyboard.
ABC|Show the software keyboard.
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_close_black_18dp.png">|Hide the keypad.

<br><br>
[HOME](index.md)　[Operators and Functions](operator_and_function.md)　[Settings](settings.md)　  
