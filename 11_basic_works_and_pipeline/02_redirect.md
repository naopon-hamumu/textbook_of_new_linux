### 02 リダイレクト
- 標準入力のリダイレクト
  ```
  $ <コマンド> < <ファイル名>
  ```

- 標準出力のリダイレクト<br>
  - コマンドの結果をファイルに保存
    ```
    $ <コマンド> > <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/b11503cb4a91b35ca7a12451bcc2e16e.png)](https://gyazo.com/b11503cb4a91b35ca7a12451bcc2e16e)

- 標準エラー出力
  - エラーメッセージをファイルに保存
    ```
    $ <コマンド> 2> <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/aeb4d9e4ac5ecd639478f973d06b9b90.png)](https://gyazo.com/aeb4d9e4ac5ecd639478f973d06b9b90)

    - 2つのファイルにリダイレクトする
      ```
      $ <コマンド> > <ファイル名1> 2> <ファイル名2>
      ```
      [![Image from Gyazo](https://i.gyazo.com/0b60ecf14e93a2060104320c0c27ada4.png)](https://gyazo.com/0b60ecf14e93a2060104320c0c27ada4)<br>

      * ファイル1 => 実行結果
      * ファイル2 => エラーメッセージ

- 標準出力と標準エラー出力をまとめる
  - 標準出力と標準エラーをまとめてリダイレクト
    ```
    $ <コマンド> > <ファイル名1> 2>&1
    ```
    [![Image from Gyazo](https://i.gyazo.com/143735c50f734abb6fff0e313631fde1.png)](https://gyazo.com/143735c50f734abb6fff0e313631fde1)

    * 標準入出力の数値
      | 数値 | 入出力チェネル |
      | :---: | :--- |
      | 0 | 標準入力 |
      | 1 | 標準出力 |
      | 2 | 標準エラー出力 |

- リダイレクトによる上書き
  - リダイレクトによる既存のファイル上書き
    ```
    $ <コマンド> > <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/4c13572679812eee66937accbb4d20f2.png)](https://gyazo.com/4c13572679812eee66937accbb4d20f2)

  - 追記リダイレクトで既存ファイルを上書きしない
    ```
    $ <コマンド> >> <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/456e17641ff37c3c9f0be43eb955f405.png)](https://gyazo.com/456e17641ff37c3c9f0be43eb955f405)

- リダイレクトの記法
  | 記号 | 内容 |
  | :---: | :--- |
  | < FILE | 標準入力をFILEに変更する |
  | > FILE | 標準出力をFILEに変更する |
  | >> FILE | 標準出力の出力をFILEの末尾に追記する |
  | 2> FILE | 標準エラー出力をFILEに変更する |
  | 2>> FILE | 標準エラー出力の出力をFILEの末尾に追記する |
  | > FILE 2>&1 | 標準出力と標準エラー出力を、共にFILEに変更する |
