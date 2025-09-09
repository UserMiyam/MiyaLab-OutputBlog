
-----

### MiyaLab-OutputBlog へようこそ！

MiyaLab-OutputBlogは、HugoとGitHub Pagesを利用して構築された、技術学習の記録と共有を目的とした技術ブログです。

-----

### 環境構築とサイト運用

このプロジェクトをローカルで動かすには、以下の環境が必要です。

  - **Hugo**: [公式サイト](https://gohugo.io/)からインストールしてください。
  - **Git**: [公式サイト](https://git-scm.com/)からインストールしてください。

#### 1\. プロジェクトのセットアップ

まず、リポジトリをクローンし、プロジェクトの基本設定を行います。

```sh
# リポジトリをクローン
git clone https://github.com/UserMiyam/MiyaLab-OutputBlog.git

# プロジェクトフォルダに移動
cd MiyaLab-OutputBlog
```

#### 2\. Hugoサイトの設定

このリポジトリにはHugoの設定ファイルが含まれていないため、手動で追加します。

1.  `MiyaLab-OutputBlog`フォルダのルートに、\*\*`hugo.toml`\*\*という名前のファイルを作成します。

2.  作成した`hugo.toml`をエディタで開き、以下の内容をコピー＆ペーストしてください。

   ```toml
  baseURL = 'http://example.org/'
  languageCode = 'ja-jp'
  title = 'あなたのブログのタイトル'
  theme = 'hugo-book'
  ```

#### 3\. テーマの追加

サイトの見た目を決めるテーマをインストールします。ここでは**hugo-book**テーマを使用します。別のテーマを使いたい場合は、URLとテーマ名を置き換えてください。

```sh
# テーマをGitのサブモジュールとして追加
git submodule add https://github.com/alex-shpak/hugo-book.git themes/hugo-book
```

#### 4\. ローカルでの実行

すべての設定が完了したら、ローカルサーバーを起動してサイトを確認します。

```sh
hugo server -D
```

サーバー起動後、ブラウザで **http://localhost:1313/** にアクセスすると、サイトが表示されます。

#### 5\. GitHubへの公開

変更をGitHubに反映させるには、コミットしてプッシュします。

```sh
# すべての変更をステージング
git add .

# コミットメッセージを付けてコミット
git commit -m "feat: Initial commit of Hugo site"

# GitHubへプッシュ
git push -u origin main
```


-----
