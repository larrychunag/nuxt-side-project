# nuxt atomtic design Todolist 実装

## Todolist

### atom

- Button
- Card

### moleculars

- Edit/Deleted Card


### ディレクトリ構成
```
/public: /src/publicのファイルがコピーされる
/src
 + /components
    + /atoms コンポーネントの最小単位
    + /containers templateをラップするためのコンポーネント（react-query使用時に必要）
    + /layout レイアウト用コンポーネント
    + /organisms 複数のコンポーネントを組み合わせて作るコンポーネント 例）検索フォーム(テキストフォーム + 検索ボタン) 
    + /templates 各コンポーネントを呼び出す親となるコンポーネント。pageファイル毎に作成する
```
