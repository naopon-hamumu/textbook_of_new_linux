### 06 tailコマンド ー末尾部分を表示する
- tailコマンド<br>
  デフォルトは10行
  ```
  $ tail <ファイル名>
  ```
  [![Image from Gyazo](https://i.gyazo.com/f565bcf9b3301ee8238cd6c633c638d8.png)](https://gyazo.com/f565bcf9b3301ee8238cd6c633c638d8)

  - 行数を指定する場合
    ```
    $ tail -n <行数> <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/29dfd69f00f87bd386d8522c3d3f9d94.png)](https://gyazo.com/29dfd69f00f87bd386d8522c3d3f9d94)

  - ファイルへの追記を監視する
    ```
    $ tail -f <ファイル名>
    ```
    [![Image from Gyazo](https://i.gyazo.com/08ce0d23a3d591a29d0b3b8a2070b705.png)](https://gyazo.com/08ce0d23a3d591a29d0b3b8a2070b705)
