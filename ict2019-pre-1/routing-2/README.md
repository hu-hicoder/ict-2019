# 外に出れません・・。[ルーティング]
## 問題概要
```
あなたは新しくルーターを購入しました。そして、新しく購入したルーターを自分の部屋に設置しました。
新しいルーターは、元々家にあったルーターの配下に接続されています。(2重ルーターの状態です。)
新しく購入したルーターに自分のPCを接続しましたが、なぜかInternetと通信ができません。
外部Internetと通信ができる状態にしてください。 
```
- 全文は https://blog.icttoracon.net/2019/09/01/ictsc2019-一次予選-問題解説-外に出れません・・。/ を見てください

## 登場する技術
- VyOS
- ルータ
- NATとSNATとDNAT

## 参考になりそうな資料
- https://ja.wikipedia.org/wiki/%E3%83%AB%E3%83%BC%E3%82%BF%E3%83%BC / ルータ 
- https://wiki.vyos.net/wiki/NAT / VYOS、NATの設定について
- https://yoru9zine.hatenablog.com/entry/2015/12/19/072304 / NATとSNATとDNAT 

## どう手を動かしたらいいか
- ルータの構成を理解する必要がある
- 後はSNAT命!!!!! 