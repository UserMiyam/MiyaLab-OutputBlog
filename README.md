# MiyaLab-OutputBlog
MiyaLab-OutputBlogは技術の学習を棚卸するためにHugoとGitHub Pagesで構築されたサイトです。

Hugo,Git　install完了済みであること。

・リポジトリをクローン
git clone https://github.com/UserMiyam/MiyaLab-OutputBlog.git
cd MiyaLab-OutputBlog

 ・Hugoサイトの設定
 ※クローンしたリポジトリにはHugoの設定ファイルが含まれていないため、手動で追加します。
 MiyaLab-OutputBlogフォルダのルートに、hugo.tomlという名前のテキストファイルを作成

hugo.tomlをエディタで開き、以下の内容をコピー＆ペースト
 baseURL = 'http://example.org/'
languageCode = 'ja-jp'
title = 'あなたのブログのタイトル'
theme = 'hugo-book'

・テーマをGitのサブモジュールとして追加
git submodule add https://github.com/alex-shpak/hugo-book.git themes/hugo-book

・ローカル環境実行
 hugo server -D

・変更をコミットしてGitHubにプッシュ
 git add .
git commit -m "feat: Initial commit of Hugo site"
git push -u origin main
