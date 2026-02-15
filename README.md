## 更新手順（ローカルプレビュー）

### 必要環境
- Hugo extended v0.155.3

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
### ニュース（/posts/）の追加
#### ファイルを追加
```bash
hugo new posts/yyyy-mm-dd-something.md
```
- content/posts/yyyy-mm-dd-*.md が作られる
  - cover.images は static/img/posts/* に置く

#### コミット
```bash
git commit -m "Add yyyy-mm-dd-*.md"
```

### ローカルでプレビュー
```bash
# デフォルトポートは 1313
hugo server

# スマホなど外部端末からアクセスする場合
hugo server --bind 0.0.0.0 --baseURL http://[ip_address]:1313
```

### 外部サイトに反映
```bash
git push
```
- 反映されない場合，アクションが失敗していないか確認する
  - https://github.com/inetlab-yamanashi/inetlab-yamanashi.github.io/actions