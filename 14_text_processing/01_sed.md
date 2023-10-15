### 01 sedコマンド ーストリームエディタ
- sedコマンドの形式
  ```
  $ sed [オプション] <スクリプト> <対象ファイル>
  ```

  - 行を削除する
    ```
    $ sed <行>d <対象ファイル>
    ```
    [![Image from Gyazo](https://i.gyazo.com/b3dd0188a388933e80aa0947e60ece8f.png)](https://gyazo.com/b3dd0188a388933e80aa0947e60ece8f)

  - 行を表示する
    ```
    $ sed <行>p <対象ファイル>
    ```
    [![Image from Gyazo](https://i.gyazo.com/38fb86abfd9d1b09ac68ce71bc579f48.png)](https://gyazo.com/38fb86abfd9d1b09ac68ce71bc579f48)

    * 特定の行だけを表示
      ```
      $ sed -n <行>p <対象ファイル>
      ```
      [![Image from Gyazo](https://i.gyazo.com/f635e31c17d50aa16006a247ceebcbb8.png)](https://gyazo.com/f635e31c17d50aa16006a247ceebcbb8)

  - 行を置換する
    ```
    $ sed 'アドレスs/置換前文字列/置換後文字列/フラグ' <対象ファイル>
    ```
    [![Image from Gyazo](https://i.gyazo.com/1545be8da61d6260561c2d5ab43b8372.png)](https://gyazo.com/1545be8da61d6260561c2d5ab43b8372)

    * 見つかった全ての文字列を置換
      ```
      $ sed 's/置換前文字列/置換後文字列/g' <対象ファイル>
      ```
      [![Image from Gyazo](https://i.gyazo.com/5c1d958d19c2c161a747ec3d503804fd.png)](https://gyazo.com/5c1d958d19c2c161a747ec3d503804fd)

    * 置換が発生した行だけを表示する
      ```
      $ sed -n 's/置換前文字列/置換後文字列/gp' <対象ファイル>
      ```
      [![Image from Gyazo](https://i.gyazo.com/eb9af237bed1387725eba58804874499.png)](https://gyazo.com/eb9af237bed1387725eba58804874499)
