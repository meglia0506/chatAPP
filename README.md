# chatAPP

## なぜ作ろうとしているのか
先日ゲーム科の学校の先生に、ゲームサーバに関する知識をつけたいと相談したところ  
「最近TCPでかなり作ってるし複数人で使えるチャットサーバー辺り作ってみたら良いよ、ノンブロッキングとかも勉強してきて」  
とお声を頂いたので作ることにしました。  

## 仕様
### クライアント
ノンブロッキングを勉強しておいでと聞いているのでソケットをselectで監視し、受信を行う。
言語はGUIの関係でC#が有力
ノンブロッキングモードで自力で書くべきなのかはまだ良くわかっていない（そのうち書きます)  
追記3/6　とりあえずpython(CUI)で書きました

### サーバー
コネクション数が増えていくのでとりあえずforkでの処理を勉強してみようかと  
~~言語はPHPの予定(ワンチャンCPP)~~男気CPP決めます(深夜テンション)  
追記3/6  MySQLやらsqlite辺り使えば割と簡単にできそうだが使いたくないしforkだけで実装するのは（主にプロセス間通信が)苦痛すぎるのでPHPやめます、EPOLLさんはまたの機会に
