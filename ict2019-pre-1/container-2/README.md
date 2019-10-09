# 監視できない！[コンテナ]
## 問題概要
```
kubernatesのクラスタの情報を取得するnotifierというアプリケーションを作った。これは、自身がデプロイされたクラスタのPodに関するイベントを外部のサーバにwebhookする機能を持つ。そのアプリケーションからイベントが見れないので、イベントを見れるようにする。
```
- 全文は https://blog.icttoracon.net/2019/08/28/ictsc2019-%e4%b8%80%e6%ac%a1%e4%ba%88%e9%81%b8-%e5%95%8f%e9%a1%8c%e8%a7%a3%e8%aa%ac-%e7%9b%a3%e8%a6%96%e3%81%a7%e3%81%8d%e3%81%aa%e3%81%84%ef%bc%81/ を見てください。

## 登場する技術
- kubernates(kubectl)
- yaml

## 参考になりそうな情報
- https://kubernetes.io/docs/home/ kubernates document
- https://qiita.com/suzukihi724/items/241f7241d297a2d4a55c

## どう手を動かしたらいいか
- kubernatesをそんなに使ったことがないのでわからない。ここは、SpringBootのやつを思い出してそいつを使うか
- kubernatesが必要とされている背景とか理解したい。