### 01 ファイルを探す
- ディレクトリツリーからファイルを探す
  ```
  $ find <検索開始ディレクトリ> <検索条件> <アクション>
  ```
  [![Image from Gyazo](https://i.gyazo.com/841aa8a745a247d403b2c9afdd993b16.png)](https://gyazo.com/841aa8a745a247d403b2c9afdd993b16)

  - ファイル名で探す
    * -name：大文字と小文字を区別する
    * -iname：大文字と小文字を区別しない<br>
    ※ ワイルドカードを使用する場合は以下のようにする<br>
      [![Image from Gyazo](https://i.gyazo.com/1279c569b8509b4aa3b81e2a12552523.png)](https://gyazo.com/1279c569b8509b4aa3b81e2a12552523)

  - ファイルの種類で探す<br>
    | 指定 | ファイル種別 |
    | :---: | :--- |
    | -type f | 通常ファイル |
    | -type d | ディレクトリ |
    | -type l | シンボリックリンク |

    [![Image from Gyazo](https://i.gyazo.com/961473d5deb3c11ae4ae0a6846ea16cd.png)](https://gyazo.com/961473d5deb3c11ae4ae0a6846ea16cd)

  - 複数の検索条件の指定
    ```
    $ find <検索開始ディレクトリ> <検索条件1> -a <検索条件2> <アクション>
    $ find <検索開始ディレクトリ> <検索条件1> <検索条件2> <アクション>
    ```
    [![Image from Gyazo](https://i.gyazo.com/774f5168878e673ac675685295f2b970.png)](https://gyazo.com/774f5168878e673ac675685295f2b970)<br>
    [![Image from Gyazo](https://i.gyazo.com/eed0f7afdceaf6f5b7e3bbc69e5de68f.png)](https://gyazo.com/eed0f7afdceaf6f5b7e3bbc69e5de68f)

- ファイル名データベースからファイルを探す
  ```
  $ locate <ファイル名>
  ```
  [![Image from Gyazo](https://i.gyazo.com/d6b5158a76bd760bdd9f2d78bc8e0407.png)](https://gyazo.com/d6b5158a76bd760bdd9f2d78bc8e0407)

  - 大文字小文字を無視して検索
    ```
    $ locate -i <ファイル名>
    $ locate --ignore-case <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/a8e9680ac87d71926c34b37cebcb80be.png)](https://gyazo.com/a8e9680ac87d71926c34b37cebcb80be)
  
  - ファイル名だけを対象に検索
    ```
    $ locate -b <ファイル名>
    $ locate --basename <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/e319ef881977203a4b1787d86116d9dc.png)](https://gyazo.com/e319ef881977203a4b1787d86116d9dc)
  
  - 複数検索（OR）
    ```
    $ locate <ファイル名> <ファイル名>
    ```
  
  - 複数検索（AND）
    ```
    $ locate -A <ファイル名> <ファイル名>
    ```
