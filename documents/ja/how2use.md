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
入力を取り消す|直前の入力を取り消して元に戻します。誤って全削除した場合などに使用することを想定しており、最大で10操作前まで戻ることが可能です。
式を整形|編集中の式を整形して見やすくします。
設定|[設定画面](settings.md)に遷移します。
オンラインヘルプ|このヘルプページをデフォルトのブラウザで開きます。
下書き|下書きの一覧が表示されます。選択すると下書きを開きます。<br>ゴミ箱のアイコンをタップすると下書きを削除できます。
保存済みファイル|名前を付けて保存したファイルの一覧が表示されます。選択するとファイルを開きます。<br>ゴミ箱のアイコンをタップするとファイルを削除できます。

## <a name ="lineno">行番号と行参照</a>
行番号をタップするとその行の答えを参照するための変数 `${LineNo}` が入力されます。参照変数は複雑な計算を簡単な式に分割して計算する時に便利です。改行の入力によって参照している行番号が変わった場合は、参照変数も自動的に更新されます。現時点では参照できる行は前の行のみになります。例えば5行目に `$6` と書いても6行目を参照することはできません。

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/line_no.png">

## 編集領域
ここに計算式を書くことでリアルタイムで結果領域の答えが表示されます。計算式は <img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_return_black_18dp.png" width="20px" align="top"> をタップして改行することで何個でも書くことができます。結果は1行毎に別々に計算され結果領域に表示されます。計算式が長い場合は自動的に折り返して表示され複数行になることがありますが、結果は1行として扱われます。計算式にエラーがある場合は答えは表示されません。  
また、編集領域には数式だけでなくメモを書くことができます。計算式と一緒にメモを残しておくことで後から式を見なおした時に、なんの計算だったか一目瞭然です。


## 結果領域と総合計領域
結果の数値をタップすると結果の2進数、16進数、消費税込、税別の金額が計算されポップアップで表示されます。それぞれの結果はタップすることでクリップボードにコピーされます。また行番号をタップすると編集領域に `${LineNo}` が入力されます。  
税込、税別表示のカッコ内には税額が表示されます。 `税込:1,080(80)` という表示は税別で`1,000円`の税込み価格は `1,080円` でそのうち`80円`が税額ということを意味しています。同様に`税別:926(74)`という表示は税込み`1,000円`の税別価格は`926円`で`74円`の消費税がかかり、合計で1,000円という意味になります。

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/result_popup1.png">
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/result_popup2.png">

## 入力パッド
**入力パッドの高さはデフォルトで、お使いの文字入力ソフトのソフトウェアキーボードの高さに合わせた高さになります。**お使いのソフトウェアキーボードがコンパクトな場合、入力パッドも小さくなり押しづらくなる可能性があります。その場合は、[設定](settings.md)で入力パッドの高さを自分で調整するか、文字入力ソフトの設定でソフトウェアキーボードの高さを調整することで改善することができます。  
入力パッドは左右にスワイプすることで、切り替えることができます。現時点では３種類の入力パッドをサポートしています。各ボタンの右下に `...` 三点リーダが表示されているボタンはロングタップすると関連するボタンがポップアップ表示されます。例えば「削除ボタン」をロングタップすると「全削除ボタン」と「1行削除ボタン」が表示されます。


<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/keypad.png">
<br>
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/popup_pad.png">
<br>
### ロングタップで表示されるポップアップ

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

### タブレットレイアウト
お使いの端末がタブレットの場合、広い画面を利用して配置されるボタンが増加します。これによりロングタップを必要としていたボタンが、１タップで入力できるようになります。

#### 7インチタブレット以上の場合
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/keypad7.png">

#### 9インチタブレット以上の場合
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/keypad9.png">

**※タブレットの画面の大きさはあくまで目安です。実際のボタン配列は解像度などによって異なります。**

### 引数入力パッド
入力をより簡素化するために、関数や`√`、`^`などを入力すると引数を入力するための入力パッドがポップアップで表示されます。

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/function_pad.png">

## パッド切替
|ボタン|説明|
|:-----------|:------------|
123|ソフトウェアキーボードを非表示にします。
ABC|ソフトウェアキーボードを表示します。
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_close_black_18dp.png">|入力パッドを非表示にします。

<br><br>
[HOME](index.md)　[演算子と関数](operator_and_function.md)　[設定](settings.md)　[カスタマイズの例](example4theme.md)　[使用例](http://android.ascii.jp/2016/02/29/893463)  
