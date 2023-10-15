### 03 uniqコマンド ー重複行を取り除く
- uniqコマンド
  ```
  $ uniq <ファイル名>
  ```
  [![Image from Gyazo](https://i.gyazo.com/27eaad3180a26b609a365720294cfa3e.png)](https://gyazo.com/27eaad3180a26b609a365720294cfa3e)

  ※ 超副業が連続してない場合には、取り除かれない
    [![Image from Gyazo](https://i.gyazo.com/e6da23e93c713081a6a5e0c51e256aba.png)](https://gyazo.com/e6da23e93c713081a6a5e0c51e256aba)

    対処法
      [![Image from Gyazo](https://i.gyazo.com/4db3cb4e759f6f92698a01dc3d96b353.png)](https://gyazo.com/4db3cb4e759f6f92698a01dc3d96b353)<br>
      [![Image from Gyazo](https://i.gyazo.com/aed1521b949029ca3cf629dfc03488b2.png)](https://gyazo.com/aed1521b949029ca3cf629dfc03488b2)

  - 重複行を数える
    ```
    $ sort <ファイル名> | uniq -c
    ```
    [![Image from Gyazo](https://i.gyazo.com/c43f39c20bcb4e90d837323ff0f09f00.png)](https://gyazo.com/c43f39c20bcb4e90d837323ff0f09f00)

    * -cオプションの結果をさらにソートして多い順に表示
      ```
      $ sort <ファイル名> | uniq -c | sort -rn
      ```
      [![Image from Gyazo](https://i.gyazo.com/9b759997d06c98e3658badf342b2ece3.png)](https://gyazo.com/9b759997d06c98e3658badf342b2ece3)

    * -cオプションの結果をさらにソートして少ない順に表示
      ```
      $ sort <ファイル名> | uniq -c | sort -n
      ```
      [![Image from Gyazo](https://i.gyazo.com/b1c7d1f56dabf69a8eaac2ac86332677.png)](https://gyazo.com/b1c7d1f56dabf69a8eaac2ac86332677)
