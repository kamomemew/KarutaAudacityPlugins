# KarutaYomiLabeling

競技かるたの音声から札が読まれている部分のみを抽出するAudacityプラグインです。

## インストール

先に[Audacity](https://www.audacityteam.org/)をインストールしてください。
また、必要ならLAMEやFFMpegの設定をしてください。

Audacityの`ツール > Nyquistプラグインをインストール`から、KarutaYomiLabeling.nyを選択してください。


## 使用方法

下記を設定します。
(一般的なかるたの取り動画などの場合にはフィルターやコンプレッサーを先にかけた方が良い結果になりやすいです。)

* しきい値のレベル

このレベルより下の音量は無音と判定します。

* 無音部の最短継続時間

読みと読みの間の間隔を指定します。通常は1秒程度

* 最短ラベル間隔

最適な値を探してください。

* Minimum Sound Duretion

この秒数以下の区間は無視されます。

* ラベル配置形式

preprocess ONLY の場合、ラベルは通常通り配置されます。
pre+postの場合にはラベルは読み開始をもとに再配置されます。(動画編集などに)

## 謝辞

このプラグインはAudacity付属のLabel Sounds(作者: Steve Daulton)を改変して製作しました。
