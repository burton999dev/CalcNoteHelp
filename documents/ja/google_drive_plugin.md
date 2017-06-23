# GoogleDriveプラグイン
[GoogleDriveプラグイン](https://play.google.com/store/apps/details?id=com.burton999.notecal.plugin.gdrive)をインストールすることでCalcNoteに自動バックアップ機能を追加することができます。この[プラグイン](https://play.google.com/store/apps/details?id=com.burton999.notecal.plugin.gdrive)はv2.4.14以降のCalcNoteの無料版とPro版の両方で利用できます。

## 初期設定
1. アプリを起動します。
1. `連絡先へのアクセス`を許可します。この権限は端末で利用可能なGoogleアカウントの一覧を取得するのに必要です。GoogleDriveプラグインではこの権限を連絡先にアクセスする目的では利用しません。
1. `Googleドライブと同期`をONにします。
1. バックアップを保存するためのGoogleアカウントを選択します。
1. 初期化処理が行われて自動バックアップが有効になります。CalcNoteでの設定は必要ありません。
1. 自動バックアップを無効にしたい場合は`Googleドライブと同期`をOFFにします。
<br/>
<br/>
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/ja/google_drive_plugin.png">

## 仕組み
[GoogleDriveプラグイン](https://play.google.com/store/apps/details?id=com.burton999.notecal.plugin.gdrive)はGoogleドライブのルートフォルダに `__calcnote__` という名前のフォルダを作成し、そのフォルダにバックアップを作成します。  
CalcNoteは`__calcnote__` フォルダ以外のフォルダ、ファイルにアクセスすることはありません。また、`__calcnote__` フォルダの配下に `trash` というフォルダを作成し、そこに削除されたファイルを保存します。

## 仕様
1. ファイルと下書きが自動的にバックアップされます。
1. バックアップはネットワーク接続が有効な時にバックグラウンドで行われます。WIFI以外の3G/4G回線使用時もバックアップ処理は行われます。
1. 複数の端末で利用した場合、端末Aで作成したファイルは、自動的に端末Bに同期されます。ファイルの更新や削除も同期されます。
1. バックアップが完了するまでタイムラグがあるので基本的に複数の端末で同じファイルを同時に編集/削除することは推奨していません。あくまで自動バックアップの用途にご利用ください。
1. 複数の端末で同じファイルを更新した場合、より新しい変更が有効になります。端末の時刻設定がズレていると意図しない動作になる可能性があります。
1. CalcNoteが保存した以外のファイルは無視され同期されません。例えば他のアプリで__calcnote__フォルダにファイルを作成しても、そのファイルは同期されず無視されます。
1. 削除したファイルはtrashフォルダに移動され残り続けます。必要に応じて手動で削除してください。

<br><br>
[HOME](index.md)　[基本操作](how2use.md)　[文法](http://burton999dev.github.io/CalcNoteHelp/grammar_ja.html)　[演算子と関数](operator_and_function.md)　[単位変換](unit_converter.md)　[通貨変換](currency_converter.md)　[フローティングウィジェット](floating_widget.md)　[設定](settings.md)　[キーパッドのカスタマイズ](customizing_keypad.md)　[カスタマイズの例](example4theme.md)　[ユーザー拡張機能](custom_extension.md)　[FAQ](faq.md)　[使用例](http://android.ascii.jp/2016/02/29/893463)  

