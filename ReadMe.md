# このソフトウェアについて #

GiHubApi.Repositories.Create.201610140807は私個人が学習目的で作成したソフトウェアである。

curlでGitHubAPIを実行してリモートリポジトリを生成するバッチファイル。

# 開発環境 #

* Windows XP Pro SP3 32bit
    * cmd.exe
* curl.exe
    * 7.24.0

## WebService ##

* [GitHub](https://github.com/)

# 手順

## 準備

1. [GitHubアカウントを取得すること](https://github.com/join)
1. [AccessTokenを取得すること](https://github.com/settings/tokens)

以上でこのバッチで使うユーザ名とAccessTokenを取得できる。

## リポジトリ作成

1. リモートリポジトリにしたい名前のディレクトリを用意する（名前に使える文字は半角英数字と`.`,`_`,`-`だけ）
1. ディレクトリに今回のbatファイルを入れる
1. `start.bat`をテキストエディタで開く
1. `GITHUB_USER`にユーザ名、`GITHUB_USER`にAccessTokenをセットする
1. `REPO_DESC`に説明文、REPO_HOMEに任意のURLをセットする
1. CP932(Shift-JIS)で保存する
1. `start.bat`をダブルクリックして実行する
1. GitHubにリモートリポジトリができていることを確認する

## push

このバッチの内容には直接関係ないが、リモートリポジトリにgitからpushするためには、SSH鍵を作成し、GitHubへ公開鍵を設定する必要がある。[手順](http://ytyaru.hatenablog.com/entry/2016/06/17/082230)

なお、[前回](https://github.com/ytyaru/CreateRepository201610012001)`git init`から`git push`までバッチファイルにしたものがある。

# ライセンス #

このソフトウェアはCC0ライセンスです。

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.ja)
