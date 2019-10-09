# 郷に入っては郷に従え[パケットフィルタ]
## 問題概要
```
公開したコンテナのWebサーバの設定を直し、aptコマンドを使用できるようにする
```
- 全文は https://blog.icttoracon.net/2019/08/28/ictsc2019-一次予選-問題解説-郷に入っては郷に従え/ を見てください

## 登場する技術
- LXC(lxc config)
- apache
- iptables
- DNAT
- VNC
- nginx

## 参考になりそうな情報
- http://ipset.netfilter.org/iptables.man.html iptables manpage
- https://knowledge.sakura.ad.jp/2108/ LXC導入
- https://linuxcontainers.org/ja/lxc/introduction/ LXCについて
## どう手を動かしたらいいか
- iptablesに触ってみる。実機は危険かもしれないので、Webサービス作るノリでやってみる？これもVM上でやるほうがいいのかもしれない。
- proxyとかを理解していないと難しそう