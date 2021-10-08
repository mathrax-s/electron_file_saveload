# Electron + p5js (File Save & Load)

Electron（Electron Fiddleではありません）とp5jsをつかった、JSONファイルのセーブとロードができるサンプルです。アプリケーションの設定をセーブ・ロードすることを想定しています。


<img src = "./screenshot_01.png"></img>

JSONファイルは、同階層の「pref.json」という名前にしてあります。このファイルをロードするときに、ファイルの存在を確認してから、存在しなければデフォルトの値で新規作成するようにしています。

ファイルの存在を確認する部分がp5jsにはなかったので、nodejaのpathモジュールとfsモジュールを使って作っています。