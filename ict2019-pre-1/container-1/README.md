# コンテナが作れない[コンテナ]
## 問題概要
```
Dockerで学内CTFサーバを構築したが、 docker-compose build が失敗するので、 http://192.168.0.1/index にアクセスしたときにスコアボードが正常に表示されるようにDockerfileに変更を加える。
```
- 全文は https://blog.icttoracon.net/2019/08/27/ictsc2019-%e4%b8%80%e6%ac%a1%e4%ba%88%e9%81%b8-%e5%95%8f%e9%a1%8c%e8%a7%a3%e8%aa%ac-%e3%82%b3%e3%83%b3%e3%83%86%e3%83%8a%e3%81%8c%e4%bd%9c%e3%82%8c%e3%81%aa%e3%81%84/ を見てください

## 登場する技術
- Docker(Dockerfile, docker-compose.ymlの読み方)
- MySQL
- Redis
- golang
- busybox

## 参考になりそうな資料
- https://docs.docker.com/engine/reference/builder/ 公式Docker reference
- https://qiita.com/minamijoyo/items/711704e85b45ff5d6405 Docker MultiStage Build

## どう手を動かしたらいいか
- そもそもDockerをよく知らないのでMultiでイメージサイズ削減と言われても嬉しさが分からない
- とりあえず何か作ってみるか 小さくはgolangのDockerから、大きくしてSQLとの連携とか