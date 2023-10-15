### 04 フィルタ
- 標準出力の先頭10行を表示
  ```
  $ head <コマンド>
  ```

  [![Image from Gyazo](https://i.gyazo.com/5c6735eb9124f628b6b8de04295c12e2.png)](https://gyazo.com/5c6735eb9124f628b6b8de04295c12e2)<br>
  [![Image from Gyazo](https://i.gyazo.com/c4ca383ecadd1d3064a8e534f6dfc9f6.png)](https://gyazo.com/c4ca383ecadd1d3064a8e534f6dfc9f6)

- 代表的なフィルタコマンド
  | コマンド | 役割 |
  | :---: | :--- |
  | cat | 入力をそのまま出力する |
  | head | 先頭の部分を表示する |
  | tail | 末尾の部分を表示する |
  | grep | 指定した検索パターンに一致する行だけを表示する |
  | sort | 順番に並べ替える |
  | uniq | 重複した行を取り除く |
  | tac | 逆順に出力する |
  | wc | 行するやバイト数を出力する |

- 指定したファイルやディレクトリの使用容量を表示する
  ```
  $ du [オプション] <ファイル・ディレクトリ名>
  ```

  - ファイルサイズを表示
    ```
    $ du -b <ファイル名>
    ```

  - ファイルサイズの小さい順に表示
    ```
    $ du -b <ファイル名> | sort -n
    ```

  - ファイルサイズの大きい順に表示
    ```
    $ du -b <ファイル名> | sort -n | tac
    ```

  - ファイルサイズの大きい上位5つを表示
    ```
    $ du -b <ファイル名> | sort -n | tac | head -n 5
    ```
