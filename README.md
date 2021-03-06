# ShoppingOrderApp
買い物依頼アプリ（勉強用）

## 目的
- 外に出ている人に対して「帰りにこれ買ってきて！」と言う依頼を行うためのツールです。
- 特に相手がいない場合は自分用メモとしての利用を想定しています。

## 作った目的
- スタンドアロンアプリを作成、公開する練習のため
- C#の勉強のため

## 動作環境
Windows10 64bitのみ動作確認ができています。

## 使い方
### Config画面でメールアドレスの設定を行います。
細かい内容は以下の通り。
- 送信者名
  - アドレス帳に登録されていない場合に表示される項目
- 送信アドレス
  - ユーザアドレスと同一にしておけば間違いないです
- 宛先
  - メール本文の最初に [宛先]へ と表示されます
- 宛先アドレス
  - メール送信相手
- 件名
  - メール件名
- SMTPサーバー、SMTPポート、SSL通信
  - 使用しているサービスによって切り替えてください
- ユーザアドレス
  - 送信元メールアドレス
- パスワード
  - 送信元メールアドレス用パスワード
- Yahoo設定ボタン
  - Yahooメールで送る場合のSMTPサーバー、SMTPポート、SSL通信を入力します
- Google設定ボタン
  - Gmailで送る場合のSMTPサーバー、SMTPポート、SSL通信を入力します

### Start画面で詳細を入力します。
左列に品名を、右列に数量や備考を記入してSendを押すと、
Config画面で設定した宛先にメールが届きます。
なお左列に入力した行のみ送信され、右列の入力は任意となっています。

メール本文例は以下の通りです。
```
[宛先]へ

買い物依頼リストです。
=================
牛乳：2本
冷凍食品
ほうれん草：1袋
アイス：チョコ味
=================
以上、よろしくお願いします。

※：このメールはアプリから自動送信されています。
```

## 削除について
レジストリは弄っていないはずなので、
Configファイルとダウンロードしたフォルダを消してください。

## Configファイルの保存パスが分からない
C:\Users\[ユーザー名]\AppData\Local\ShoppingOrderApp
にあると思います。

## 開発環境
- OS：Windows10 64bit Home Edition
- 言語：C#
- IDE：Visual Studio 16.11.4

## LINEなどで連絡した方が早い
作り出してようやく気付きました。
せめてスマホアプリ化したほうが良かったですが、折角なので完成させました。
