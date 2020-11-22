## 概要
下記、秋葉原会の初回手順になります

### 初期設定

##### 状態確認
```console
$ git config --global user.email "{gitのmail address}"
$ git config --global user.name "{プッシュしたいファイル名、UTF-8で作成}"
```

### 作業手順
#### １．GitHuB　アカウント登録

#### ２．Discord　アカウント登録

#### ３．Git Bash　インストール

#### ４．自己紹介叩き台文面作成
　参考：Markdown記法　https://qiita.com/tbpgr/items/989c6badefff69377da7

#### ５．Git Bash　及び　GitHub　にて下記操作を実施

##### Git Bashを起動し、{自分のPC名}に移動
```console
$ cd C:\Users\{自分のPC名}
```

##### git用ディレクトリを自分のPCに作成
```console
$ mkdir github
```

##### C:\Users\{自分のPC名}　に　.ssh　というフォルダを作成

##### ディレクトリ　.ssh　に移動
```console
cd .ssh
```


##### SSH鍵　作成
```console
$ ssh-keygen -t rsa -b 4096 -C {gitのmail address} -f id_rsa
```

##### ディレクトリ　git　に移動
```console
$ cd git
$ cd repo
```

##### git クローンを実施
```console
$ git clone git@github.com:{gitのusername}/akihabara-mokumoku.git
```

##### チェックアウトを実施
```console
$ git checkout -b hase1120
```

##### 状態確認
```console
$ git status
```

##### ブランチを作成　及び　切替
```console
$ cd akihabara-mokumoku/
$ git checkout -b hase1120
```

Switched to a new branch 'hase1120'　　の表示を確認

##### 変更をステージングを実施
```console
$ git add mokumoku/2020/1122/hase-k.md
```

##### ステージングされてるファイルの差分を表示
```console
$ git diff--cached
```

##### 再確認
```console
$ git status
```

##### コミットを実施
```console
$ git commit
```

##### 自分のブランチ名でプッシュを実施
```console
$ git push origin {自分のブランチ名}
```
