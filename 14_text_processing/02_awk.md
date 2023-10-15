### 02 awkコマンド ーパターン検索・処理言語
- awkコマンドの形式
  ```
  $ awk 'パターン {アクション}' <ファイル名>
  ```

  - printとフィールド変数<br>
    * lsコマンドの結果から、5列目と9列目を表示<br>
      [![Image from Gyazo](https://i.gyazo.com/c9534e9f6fb88dc807bdeb6fd55f1e43.png)](https://gyazo.com/c9534e9f6fb88dc807bdeb6fd55f1e43)

  - パターンの指定<br>
    * ファイル名がcpで始まる行のみを対処とする<br>
      [![Image from Gyazo](https://i.gyazo.com/a464a5c99af83fab224a0d8f7b3b0208.png)](https://gyazo.com/a464a5c99af83fab224a0d8f7b3b0208)

    * 行の先頭がlで始まる行のみを対象とする<br>
      [![Image from Gyazo](https://i.gyazo.com/d2c804804f00ae06f8938917ace6e538.png)](https://gyazo.com/d2c804804f00ae06f8938917ace6e538)

- 実践例
  - 区切り文字を,に指定<br>
    [![Image from Gyazo](https://i.gyazo.com/6b148ec6f90b9879acb8862feb657580.png)](https://gyazo.com/6b148ec6f90b9879acb8862feb657580)

  - 最終フィールドの点数を表示<br>
    [![Image from Gyazo](https://i.gyazo.com/10a65524382243e59367ce006d21651c.png)](https://gyazo.com/10a65524382243e59367ce006d21651c)

  - 点数の総和を表示<br>
    [![Image from Gyazo](https://i.gyazo.com/c6666435b4c3ad8efff14b908f54d265.png)](https://gyazo.com/c6666435b4c3ad8efff14b908f54d265)

  - 平均値を表示<br>
    [![Image from Gyazo](https://i.gyazo.com/15ed5f35c11a969fca958ec32457153e.png)](https://gyazo.com/15ed5f35c11a969fca958ec32457153e)

  - awkスクリプトを保存しておき、再利用する
