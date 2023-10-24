### シェルスクリプトを配置する

```
$ mkdir ~/bin
$ mv homesize.sh. ~/bin
```

- サーチパスに~/binを追加
  ```
  $ PATH="$PATH:~/bin"
  ```

- 配置した後に有効にする
  - source
    ```
    $ source 相対パス
    ```
  - 再ログイン

- sourceコマンドでのサーチパス探索をやめさせる
  ```
  $ shopt -u sourcepath
  ```
