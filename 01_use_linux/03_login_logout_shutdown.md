### 03 ログイン、ログアウト、シャットダウン
- ログアウト
  ```
  $ exit
  ```

- シャットダウン
  シャットダウンはrootユーザのみが実行可能
  ```
  $ su
  # shutdown -h now
  ```
  - Ubuntuの場合
    ```
    $ sudo shutdown -h now
    ```
  - 再起動
    ```
    # shutdown -r now
    ```
    ```
    # /sbin/shutdown -h now
    ```
