### 02 bashのオプション
- setコマンド：オプションのオン・オフを指定
  ```
  $ set -o/+o <オプション名>
  ```
  - -o：オン
  - +o：オフ

  | オプション名 | 内容 |
  | :---: | :--- |
  | ignoreeof | Ctrl + Dを押してもシェルを終了しない |
  | noclobber | すでに存在するファイルをリダイレクトで上書きしない |
  | noglob | パス名展開を無効にする。\*などはシェルに解釈されず、そのまま\*となる |

  [![Image from Gyazo](https://i.gyazo.com/68694093cbcb6013f2dd670c03958360.png)](https://gyazo.com/68694093cbcb6013f2dd670c03958360)

- shoptコマンド：オプションのオン・オフを指定
  ```
  $ shopt -s/-u <オプション名>
  ```
  - -s：オン
  - -u：オフ

  | オプション名 | 内容 |
  | :---: | :--- |
  | autocd | ディレクトリ名のコマンドを実行すると、それがcdコマンドの引数に指定されたものとして実行される |
  | dotglob | *や?を使ったポス名展開の結果に、.で始まるファイルも含める |
  | cdspell | cdコマンド実行時、ディレクトリのちょっとしたミスタイプが自動修正される |
  | globstar | パス名展開で**というパターンを使うと、サブディレクトリまで含めた全てのファイルにマッチする |
  | histappend | bashを終了するとき、履歴ファイルにコマンドの履歴を追記し、上書きしない |

  [![Image from Gyazo](https://i.gyazo.com/ae208ab655a9926950fd62703ce0cb8d.png)](https://gyazo.com/ae208ab655a9926950fd62703ce0cb8d)
