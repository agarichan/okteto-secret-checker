# okteto-secret-checker

okteto のデプロイリンクを踏んでしまったら secret が漏洩する可能性があるのかチェックする

## デプロイボタン

！注意！自身の okteto 環境に勝手にこのリポジトリの内容がデプロイされます

<a href="https://cloud.okteto.com/deploy?repository=https://github.com/agarichan/okteto-secret-checker&branch=main">
  <img src="https://okteto.com/develop-okteto.svg" alt="Develop on Okteto">
</a>

## 実験

okteto のシークレットに  
key を SECRET、value に適当な値を入れてみる

```
deploy:
  - env
```

とりあえず、env で環境変数を表示してみる

```
installerSECRET=***
```

取得はできるが、Web コンソールの Logs では表示できない。  
これはどうせ自分しか見れないので問題ない。
