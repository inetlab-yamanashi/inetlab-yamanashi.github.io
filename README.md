# サイト管理メモ

## 前提
### 想定環境
- Hugo extended v0.155.3
- バージョン固定方法
  - `.github/workflows/hugo.yml` の `hugo-version`
  - `brew pin hugo`
    - `brew unpin hugo` で解除
    - `brew list --pinned` で確認

### 主なファイル
```
- content/
  - _index.md: トップページ
  - [menu]/
    - index.md
- static/
  - img/
    - [menu]/
```

## ニュース（/posts/）の追加
### ファイルを追加
```bash
hugo new posts/yyyy-mm-dd-something.md
```
- `content/posts/yyyy-mm-dd-something.md` が作られる
  - 画像は `static/img/posts/` に置き，front matter では `cover.image: "/img/posts/yyyy-mm-dd-something.png"` のように書く

### コミット
```bash
git commit -m "Add /posts/yyyy-mm-dd-something"
```

## ローカル・プレビューで確認
```bash
# デフォルトポートは 1313
hugo server

# スマホなど外部端末からアクセスする場合
hugo server --bind 0.0.0.0 --baseURL http://[ip_address]:1313
```

## GitHub Pages に反映
```bash
git push
```
- 反映されない場合，アクションが失敗していないか確認する
  - https://github.com/inetlab-yamanashi/inetlab-yamanashi.github.io/actions


## 年次メンテナンス（更新）

### 更新用ブランチ作成
```bash
git checkout -b yearly-update-2027
```

### 現状の固定値を記録
- Hugo: `.github/workflows/hugo.yml` の `hugo-version`（または `hugo version` コマンド）
- PaperMod: `git submodule status` の SHA（または themes/PaperMod のコミット）

### 現状のまま，クリーンビルド（ベースライン確認）
```bash
rm -rf public resources
hugo --minify
```

### Hugo をアップデート（ローカル）
```bash
brew unpin hugo
brew upgrade hugo
hugo version
```

アップデート後もビルドできることを確認：
```bash
rm -rf public resources
hugo --minify
```

### PaperMod 更新（submodule）
```bash
git submodule update --remote --merge
git submodule status
```

### Hugo 更新（Actions で固定値を上げる）
- `.github/workflows/hugo.yml` の `hugo-version` を新しい安定版へ

### クリーンビルド＋ローカル確認
```bash
rm -rf public resources
hugo --minify
hugo server --disableFastRender
```

### GitHub Actions でも確認（pushしてCIを見る）
```bash
git push -u origin yearly-update-2027
```

### main にマージして push
```bash
git checkout main
git merge --no-ff yearly-update-2027
git push
```

### Hugo バージョンを固定
```bash
brew pin hugo
brew list --pinned
```