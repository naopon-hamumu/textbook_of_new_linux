### 01 grepコマンドと正規表現
- 文字列を検索する
  ```
  $ grep [オプション] <検索パターン> <ファイル名>
  ```
  [![Image from Gyazo](https://i.gyazo.com/28dc42d79331ff97704025492d31b674.png)](https://gyazo.com/28dc42d79331ff97704025492d31b674)

  - 行番号付きでマッチ結果を表示
    ```
    $ grep -n <検索パターン> <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/4d9d275710ddcaecdb0898e78d490d4b.png)](https://gyazo.com/4d9d275710ddcaecdb0898e78d490d4b)

  - 大文字と小文字を区別せずに検索
    ```
    $ grep -i <検索パターン> <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/abb22e7f4a4193dcfa25db7c963438cf.png)](https://gyazo.com/abb22e7f4a4193dcfa25db7c963438cf)

  - 特定の文字列を含まない行を出力
    ```
    $ grep -v <検索パターン> <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/39a68cad41e6e1753e699ded89897ecc.png)](https://gyazo.com/39a68cad41e6e1753e699ded89897ecc)

  - lsコマンドの結果を絞る
    ```
    $ ls <ファイル名> | grep <検索パターン>
    ```
    [![Image from Gyazo](https://i.gyazo.com/6d618567e6ee497d52ba757f79e3a738.png)](https://gyazo.com/6d618567e6ee497d52ba757f79e3a738)
