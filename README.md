# latebloomer_var2_git
ハッカソンで作成した"latebloomer"というLINE Botの改良版 (gitを使用してデプロイしたバージョン)

ログイン
```
$ heroku login
```

停止・スタート
``` shell
# 停止 
$ heroku ps:scale web=0
# 再度スタート
$ heroku ps:scale web=1
#リスタート
$ heroku restart
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
$ heroku logs
# リアルタイムで確認
$ heroku logs --tail 
```
