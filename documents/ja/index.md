# 目次
- [はじめに](#introduction)
- [免責](#disclaimer)
- [Free版とPro版の違い](#version)
- [サポートについて](#support)
- [基本操作](how2use.md)  
- [文法](http://burton999dev.github.io/CalcNoteHelp/grammar_ja.html)  
- [演算子と関数](operator_and_function.md)  
- [単位変換](unit_converter.md)
- [通貨変換](currency_converter.md)
- [フローティングウィジェット](floating_widget.md)
- [設定](settings.md)  
- [キーパッドのカスタマイズ](customizing_keypad.md)
- [カスタマイズの例](example4theme.md)  
- [ユーザー拡張機能](custom_extension.md)
- [GoogleDriveプラグイン](google_drive_plugin.md)
- [FAQ](faq.md)  
- [使用例](http://android.ascii.jp/2016/02/29/893463)  
- [寄付](#donates)  

**※このヘルプには一部リリース前の新機能が含まれている可能性があります。その場合は次回リリースまでしらばくお待ち下さい。**

# <a name ="introduction">はじめに</a>
`CalcNote`はスマートフォン用に新しく設計された電卓アプリです。一般的な電卓アプリとは異なりメモを書くような感覚で計算式を書いて計算を行います。計算式が常に見えている状態なので計算ミスを簡単に発見することが可能です。式はメモ帳のようにいつでも修正することが可能です。計算式は改行することで何個でも書くことができるので、スマートフォンの大画面を使って複数の計算を同時に行うことができます。  
`CalcNote`はAndroid専用アプリです。iOSやmacOSなど他のプラットフォーム向けにリリースする予定はありません。  
iOSやmacOSには既に素晴らしいエディタ形式の電卓 [Soulver](https://www.acqualia.com/soulver/) があります。
とても素晴らしいアプリで私もmac上で毎日使っています。非常にオススメです。  
`CalcNote` を開発した動機は、Androidにこのような素晴らしい電卓アプリが存在しなかったからです。

# <a name ="disclaimer">免責</a>
本ソフトウェアの使用により生じた損害、逸失利益または第三者からのいかなる請求についても作者は一切その責任を負えませんので、あらかじめご了承ください。

# <a name ="version">Free版とPro版の違い</a>
`CalcNote`には無料でお使い頂ける [Free版](https://play.google.com/store/apps/details?id=com.burton999.notecal) と、有料の [Pro版](https://play.google.com/store/apps/details?id=com.burton999.notecal.pro) があります。どちらも電卓の機能としては全く同じですが、Free版には以下の制約があります。

- 画面上部に広告が表示されます。
- Google Analyticsが組み込まれており、どの機能がよく使われているか等、`CalcNote`の機能改善に役立つ情報を収集させていただいております。アプリ利用状況の分析以外の目的でこれらの情報を使用することはありません。(**個人情報や端末情報などプライバシーに関わる情報、編集内容等は一切収集しておりませんし、権限も要求していませんのでご安心ください**)
- [フローティングウィジェット](floating_widget.md)機能をお使いいただけません。

もしアプリを気に入っていただけましたら、Pro版の購入をご検討いただければ幸いです。  
Pro版は広告が無いことでエディタ領域を広く使うことができFree版よりも快適にお使いいただけます。

### Free版のアクセス許可
|権限|使用目的|
|:-----------|:------------|
バイブレーションの制御|ボタンタップ時にバイブを振動させるのに必要です。
ネットワーク接続の表示|広告を表示する為に必要です。
ネットワークへのフルアクセス|広告を表示する為に必要です。

### Pro版のアクセス許可
|権限|使用目的|
|:-----------|:------------|
バイブレーションの制御|ボタンタップ時にバイブを振動させるのに必要です。
ネットワーク接続の表示|アプリが強制終了した際のクラッシュレポートを送信するのに必要です。
ネットワークへのフルアクセス|アプリが強制終了した際のクラッシュレポートを送信するのに必要です。
GooglePlayライセンスの確認|Pro版のライセンス購入状態を確認するのに必要です。
他のアプリの上に重ねて表示|フローティングウィジェットを表示するのに必要です。
起動時の実行|Android起動時にフローティングウィジェットを自動起動するのに必要です。

### Free版からPro版へのアップグレード
[Free版](https://play.google.com/store/apps/details?id=com.burton999.notecal)と[Pro版](https://play.google.com/store/apps/details?id=com.burton999.notecal.pro)は異なるアプリとして提供している為、自動的に設定やデータを引き継ぐことはできません。  
データを移行するには、まずFree版を起動して[設定](settings.md)から`設定のエクスポート`および`ファイルのバックアップ`を行い。その後、Pro版と起動して`設定のインポート`および`ファイルのリストア`を実行します。


# <a name ="support">サポートについて</a>
バグや計算結果の不一致など、おかしな点を見つけた場合、また機能追加のご要望は以下のいずれかの方法でご連絡ください。

- アプリが強制終了した際に表示されるクラッシュレポートの送信
- burton9999dev@gmail.com 宛のメール
- [Twitter](https://twitter.com/#!/ComicCafeApp) でのメンション
- Github issue
- GooglePlayでのアプリのレビュー (評価はどうか穏便にお願いしますm(__)m)

要望などは実装することをお約束できませんが、可能な限り対応させていただきます。
また、バグの原因究明にご協力いただいた方にはお礼としてPro版のプロモーションコードを配布しております。

# <a name ="donates">寄付</a>
[Amazonのほしい物リスト](http://www.amazon.co.jp/registry/wishlist/336DBVUUWKOM8) を通じてアプリ開発者に寄付することができます。
