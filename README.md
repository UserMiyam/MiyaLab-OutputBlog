
-----

### MiyaLab-OutputBlog へようこそ！

MiyaLab-OutputBlogは、HugoとGitHub Pagesを利用して構築された、技術学習の棚卸を目的とした技術ブログです。 

https://usermiyam.github.io/MiyaLab-OutputBlog/

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
git submodule add [テーマのGitリポジトリURL] themes/[テーマ名]
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
hugo newコマンドはhugo.tomlを読み込み、正しくcontentフォルダを作成して記事を保存できるように-----

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
git submodule add [テーマのGitリポジトリURL] themes/[テーマ名]
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
`hugo new`コマンドの使い方をまとめた、より分かりやすいREADMEセクションを作成します。

-----

### 5\. 新しい記事の作成

Hugoで新しい記事を作成するには、`hugo new`コマンドを使用します。このコマンドは、`hugo.toml`ファイルの設定に基づいて、指定したカテゴリに記事ファイルを自動で生成します。

#### コマンドの基本構文

```sh
hugo new [カテゴリ名]/[記事のファイル名].md
```

  - **`[カテゴリ名]`**: 記事を分類するフォルダ名です。`content/`フォルダの中に作成されます。
  - **`[記事のファイル名]`**: 新しい記事のファイル名です。`半角英数字`と`ハイフン`を使うのが一般的です。

#### 実行例

以下の例では、それぞれのカテゴリに新しい記事を作成します。コマンドを実行すると、指定されたパスに記事ファイル（`my-new-post.md`）が生成されます。

  - **AtCoder カテゴリに新規作成**

    ```sh
    hugo new atcoder/my-new-post.md
    ```

      - 生成されるファイル: `content/atcoder/my-new-post.md`

  - **Paiza カテゴリに新規作成**

    ```sh
    hugo new paiza/my-new-post.md
    ```

      - 生成されるファイル: `content/paiza/my-new-post.md`

  - **Go カテゴリに新規作成**

    ```sh
    hugo new go/my-new-post.md
    ```

      - 生成されるファイル: `content/go/my-new-post.md`

#### 記事の編集

コマンド実行後、作成された`Markdown`ファイルを開き、以下の内容を編集してください。

```markdown
---
title: "あなたの記事のタイトル"
date: 2025-04-21T00:00:00+09:00
draft: false
tags: ["タグ1", "タグ2"]
categories: ["カテゴリ名"]
---

ここに記事の本文をMarkdownで記述します。
```


### 6\. サイトのビルドと公開

記事の作成・編集が終わったら、`hugo`コマンドでサイトをビルドします。

```sh
hugo
```

このコマンドを実行すると、\*\*`docs/`\*\*ディレクトリに公開用の静的サイト（HTML, CSS, 画像など）が出力されます。この`docs/`ディレクトリの内容をGitHubにプッシュすることで、GitHub Pagesを通じてサイトが公開されます。
補足：hugo.tomlファイルでpublishDir = "docs"と明示的に設定することで、Hugoはデフォルトのpublic/ではなく、docs/フォルダにファイルを生成するようになります。


承知いたしました。ご提示いただいたREADMEの`6. サイトのビルド`と`7. GitHub Actionsによる自動デプロイ`の間に、GitHub Pagesの設定に関する説明を追加します。

このセクションを追加することで、読者はGitHub上で手動で設定する必要があるステップを明確に理解できます。

---


### GitHub Pagesでの公開

GitHub Actionsによる自動デプロイを機能させるには、GitHubリポジトリ側で一度だけ設定が必要です。

1.  GitHubリポジトリの**「Settings」**タブに移動します。
2.  左側のメニューから**「Pages」**を選択します。
3.  **「Source」**のドロップダウンメニューで、`main`ブランチを選択します。
4.  次に、`/root`ではなく、**`/docs`**フォルダを公開元として指定します。
   
公開サイト：https://usermiyam.github.io/MiyaLab-OutputBlog/
修正中

この設定を保存すると、GitHub Actionsが`docs`フォルダにビルドされたファイルを自動でデプロイできるようになります。





-----

MiyaLab-OutputBlogのREADMEに、GitHub Actionsによる自動デプロイの説明を追加します。

-----

### 7\. GitHub Actionsによる自動デプロイ

このプロジェクトでは、GitHub Actionsを使用して、サイトのビルドと公開を自動化しています。これにより、あなたが記事を書いてプッシュするだけで、ブログが自動的に更新されるようになります。

#### ワークフローの仕組み

ワークフローファイル（`/.github/workflows/main.yml`）は、`main`ブランチへのプッシュを検知すると、以下のステップを自動で実行します。

1.  **Hugoのセットアップとビルド**: GitHubのサーバー上でHugoがインストールされ、`hugo`コマンドが実行されます。
2.  **GitHub Pagesへのデプロイ**: ビルドされた`docs/`ディレクトリの内容がGitHub Pagesに自動的に公開されます。

#### 設定方法

この自動デプロイ機能を利用するには、以下のファイルがすでにリポジトリに追加されている必要があります。

  - **`/.github/workflows/main.yml`**
    このファイルは、自動ビルドとデプロイの指示をGitHubに伝えます。

  - **`hugo.toml`**
    このファイルには、ビルドの出力先が`docs`ディレクトリになるように設定されています。

#### 使い方

設定が完了していれば、あなたは以下の手順でブログを更新できます。

1.  新しい記事を作成・編集します。
2.  Gitで変更をコミットし、プッシュします。

<!-- end list -->

```sh
# Hugoサイトをビルド
# hugo --cleanDestinationDir

# すべての変更をステージング
git add .

# コミットメッセージを付けてコミット
git commit -m "feat: 新しい記事を追加"

# GitHubへプッシュ
git push origin main
```

これで、GitHub Actionsが残りの作業を自動で行います。GitHubの\*\*「Actions」タブ\*\*で、デプロイの状況を確認できます。

-----

# Hugo 独自テーマ `my-custom-theme` の設定ガイド

このガイドでは、`MiyaLab-OutputBlog` リポジトリに含まれる独自テーマ `my-custom-theme` の設定とカスタマイズ方法について説明します。

## 1. テーマの構造

`my-custom-theme` は、以下の主要なディレクトリとファイルで構成されています。

```
themes/my-custom-theme/
├── layouts/
│   ├── _default/
│   │   ├── baseof.html
│   │   ├── list.html
│   │   └── single.html
│   ├── index.html
│   ├── taxonomy.html
│   └── terms.html
└── static/
    └── css/
        └── style.css (仮定)
```

- `layouts/`: サイトのHTMLレイアウトを定義するファイルが格納されています。
  - `_default/`: デフォルトのレイアウトファイル（`baseof.html`, `list.html`, `single.html`）が含まれており、サイトの基本的な構造を定義します。
  - `index.html`: トップページのレイアウトを定義します。
  - `taxonomy.html`, `terms.html`: タクソノミー（カテゴリやタグなど）の表示を定義します。
- `static/`: CSS、JavaScript、画像などの静的ファイルが格納されます。`css/style.css` のようなファイルが含まれることが一般的です。

## 2. `hugo.toml`でのテーマ指定

`my-custom-theme` を使用するには、プロジェクトのルートにある `hugo.toml` ファイルでテーマ名を指定する必要があります。`hugo.toml` を開き、`theme` の行を以下のように設定してください。

```toml
theme = 'my-custom-theme'
```

## 3. レイアウトのカスタマイズ

テーマの見た目や動作をカスタマイズするには、主に `layouts/` ディレクトリ内のファイルを編集します。

- **基本的なページレイアウト**: `layouts/_default/baseof.html` は、すべてのページの基本となるHTML構造を定義します。ヘッダーやフッターなど、サイト全体で共通する要素はここに記述します。
- **記事一覧ページ**: `layouts/_default/list.html` は、記事の一覧ページ（例: カテゴリページ、タグページ）の表示方法を定義します。
- **個別記事ページ**: `layouts/_default/single.html` は、個別の記事ページの表示方法を定義します。
- **トップページ**: `layouts/index.html` は、サイトのトップページのレイアウトを定義します。

これらのファイルを直接編集することで、サイトのデザインを自由に変更できます。

## 4. スタイルのカスタマイズ

サイトのスタイル（CSS）をカスタマイズするには、`static/css/` ディレクトリ内のCSSファイルを編集します。例えば、`style.css` に新しいCSSルールを追加することで、フォント、色、レイアウトなどを変更できます。

Hugoは、`static/` ディレクトリ内のファイルをサイトのルートにコピーするため、CSSファイルは `/<テーマ名>/css/style.css` のようなパスでアクセス可能になります。これを `layouts/partials/head.html` などで適切に読み込む必要があります。

## 5. その他の設定

- **`theme.toml`**: `themes/my-custom-theme/theme.toml` ファイルは、テーマのメタデータ（名前、作者、バージョンなど）を定義します。このファイルは主にテーマを公開する際に使用されますが、ローカルでの開発においてもテーマの情報を管理するのに役立ちます。


