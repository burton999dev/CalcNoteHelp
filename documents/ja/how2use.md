# 基本操作
`CalcNote`は電卓アプリですがメモ帳に近い外観をしていて最初は戸惑うかもしれませんが使い方はとてもシンプルです。   
ここでは基本的な操作方法を説明します。  

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/screen_description.png">

|領域|説明|
|:-----------|:------------|
行番号|行番号が表示される領域です。タップすると[行参照](#lineno)を入力することができます。<br>[設定](settings.md)で非表示にすることもできます。
編集領域|ここに式を書いて計算を行います。<br>メモ帳のように選択、全選択、コピー、切り取り、貼り付けなど柔軟な編集が可能です。
結果領域|計算結果が表示されます。結果は式を編集したタイミングでリアルタイムに計算されます。<br>結果の数字をタップすると消費税、2進数、16進数の結果が表示されます。
総合計領域|編集領域に複数の計算式を書いた場合、答えは各行毎に計算されます。それら全ての総合計が表示されます。<br>結果の数字をタップすると消費税、2進数、16進数の結果が表示されます。
入力パッド|入力パッドを左右にスワイプすることでパッドを切り替えることができます。<br>[数値入力] <-> [関数入力] <-> [ビット演算]の3つの入力パッドがあります。
パッド切替|ソフトウェアキーボードの表示、非表示、入力パッドの表示、非表示を操作できます。

## メニュー
画面右上にあるアクションメニューをタップするか、サイドメニューを表示することで`CalcNote`の様々な機能にアクセスすることができます。  

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/open_menu.png">

**サイドメニューは以下の方法で表示することができます。**  
1. 画面左上にある三本線のアイコンをタップする  
2. 画面左端から右へスワイプする  
3. ハードウェアキーのある端末で、メニューボタンを押す  

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/menu_description.png">

|メニュー|説明|
|:-----------|:------------|
新規ファイル|編集中の計算式を下書きとして保存して、新規ファイルを作成します。
保存|編集中の計算式を名前を付けて保存します。
エクスポート|編集中の計算式をクリップボードにコピーしたり、他のアプリケーションに共有することができます。
式を整形|編集中の式を整形して見やすくします。
設定|[設定画面]()に遷移します。
下書き|下書きの一覧が表示されます。選択すると下書きを開きます。<br>ゴミ箱のアイコンをタップすると下書きを削除できます。
保存済みファイル|名前を付けて保存したファイルの一覧が表示されます。選択するとファイルを開きます。<br>ゴミ箱のアイコンをタップするとファイルを削除できます。

## <a name ="lineno">行番号と行参照</a>
行番号をタップするとその行の答えを参照するための変数 `${LineNo}` が入力されます。参照変数は複雑な計算を簡単な式に分割して計算する時に便利です。改行の入力によって参照している行番号が変わった場合は、参照変数も自動的に更新されます。現時点では参照できる行は前の行のみになります。例えば5行目に `$6` と書いても6行目を参照することはできません。

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/line_no.png">

## 編集領域
ここに計算式を書くことでリアルタイムで結果領域の答えが表示されます。計算式は <img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_return_black_18dp.png" width="20px" align="top"> をタップして改行することで何個でも書くことができます。結果は1行毎に別々に計算され結果領域に表示されます。計算式が長い場合は自動的に折り返して表示され複数行になることがありますが、結果は1行として扱われます。

## 結果領域と総合計領域
結果の数値をタップすると結果の2進数、16進数、消費税込、税別の金額が計算されポップアップで表示されます。それぞれの結果はタップすることでクリップボードにコピーされます。また行番号をタップすると編集領域に `${LineNo}` が入力されます。

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/result_popup1.png">
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/result_popup2.png">

## 入力パッド
入力パッドは左右にスワイプすることで、切り替えることができます。現時点では３種類の入力パッドをサポートしています。各ボタンの右下に `...` 三点リーダが表示されているボタンはロングタップすると関連するボタンがポップアップ表示されます。例えば「削除ボタン」をロングタップすると「全削除ボタン」と「1行削除ボタン」が表示されます。


<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/keypad.png">
<br>
**ロングタップで表示されるポップアップ**  

|ボタン|ロングタップ1|ロングタップ2|
|:-----------|:------------|:------------|
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_backspace_black_18dp.png">|全削除|行削除
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_return_black_18dp.png">|`${LineNo}`|
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_arrow_left_bold_black_18dp.png">|行の先頭に移動|行の先頭まで選択
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_arrow_right_bold_black_18dp.png">|行の末尾に移動|行の末尾まで選択
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

## パッド切替
|ボタン|説明|
|:-----------|:------------|
123|ソフトウェアキーボードを非表示にします。
ABC|ソフトウェアキーボードを表示します。
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_close_black_18dp.png">|入力パッドを非表示にします。

<br><br>
[HOME](index.md)　[演算子と関数](operator_and_function.md)　[設定](settings.md)　[使用例](usecases.md)  
