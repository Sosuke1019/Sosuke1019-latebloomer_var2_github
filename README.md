# latebloomer_ver2_git
ハッカソンで作成した"latebloomer"というLINE Botの改良版 (gitを使用してデプロイしたバージョン)

ログイン
``` shell
$ heroku login
```

停止・スタート
``` shell
# 停止 
$ heroku ps:scale web=0 -a latebloomer-ver2-github
# 再度スタート
$ heroku ps:scale web=1 -a latebloomer-ver2-github
#リスタート
$ heroku restart -a latebloomer-ver2-github
```

変更
``` shell
$ git add . 
$ git commit -am "commit message"
$ git push heroku master
```

ログ出力
```shell
# 通常の確認
$ heroku logs -a latebloomer-ver2-github
# リアルタイムで確認
$ heroku logs --tail -a latebloomer-ver2-github
```
