@chashitsu/chashitsu-test-1
===========================

travis-ci.com を経由した npm パッケージの publish テストです。

- GitHub: https://github.com/chashitsu-org/chashitsu-test-1
- npmjs.com: https://www.npmjs.com/package/@chashitsu/chashitsu-test-1

### リリースフロー
1. `master` ブランチ向け Pull Request をつくる.
2. 自分以外のメンバーの誰か1人以上が approve するのを待つ.
3. テストが通ったら,  `package.json` のバージョンを上げる (patchを上げる例: `npm version patch`).
4. マージする
5. GitHub のブラウザ上から masterブランチの現在を Release する. タグ名は, `v` + バージョン名 (例: `v1.0.5).
6. (`master` ブランチの新しいタグ起因で) travis-ci が走り, 自動でpublishされる.

### コードの動作方法
``` sh
$ node ./index.js
```

### ライセンス
[CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/deed.ja)

