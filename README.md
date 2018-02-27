io-cloudからの挑戦状
====

## 概要
本リポジトリをforkした上で、問題を解いてみて下さい。  
`Linuxコマンド`の問題は、適当にファイルを作成の上、解答を記載して下さい。  
`プログラミング`の問題は、問題文の指示に従って解答して下さい。  
解答を投稿する場合は、本リポジトリにPull Requestを送信して下さい。  
分からない時は、ネットで調べながら実施して頂いて構いません

## 問題

### Linuxコマンド

1. ロードアベレージを表示しなさい

2. 空きメモリサイズを表示しなさい

3. プロセスの親子関係及びプロセス番号を表示しなさい

4. iノードの使用率を表示しなさい

5. httpリクエストを投げて、そのヘッダ情報のみ表示しなさい

6. `dir_1`ディレクトリにある拡張子logとなっているファイルに対して、ファイル毎に末尾5行分を表示させるコマンドを記載しなさい（可能であればワンライナー）

7. `dir_2`ディレクトリにあるファイルの中からファイル名が20180219から始まるファイル内に含まれる文字列`hoge`を全て`fuga`に置換するコマンドを記載しなさい（可能であればワンライナー）

8. `dir_3`ディレクトリにある`access_log`から2018/2/28 20:00～22:59までのユニーク（送信元IP）なアクセス数を出力するコマンドを記載しなさい（可能であればワンライナー）

### プログラミング

9. 以下の条件を満たすスクリプト `chk_zorome.<拡張子>` を作成しなさい
  - 条件
    - 標準入力からカンマ区切りでランダムな文字列or数値を受け取る
    - 受け取った値が、3桁の数字でない場合は、`unmach pattern: <受け取った値>`を表示する
    - 受け取った値が、3桁のぞろ目の数字であった場合は、`zorome: <受け取った値>`を表示する
    - 受け取った値が、上記に当てはまらない場合は、そのまま受け取った値を表示する
    - スクリプトの言語は、お好きにどうぞ

  - 例
    - 標準入力で受け取る値
  
      ```
      123,abc,3333,555,321
      ```

    - スクリプトの実行結果

      ```
      123
      unmatch pattern: abc
      unmatch pattern: 3333
      zorome: 555
      321
      ```

10. リポジトリ内、bak.shのコードを読んで、次の問いに答えなさい  
なお、git commitする際は、各問毎に分けて実施すること
  - bak.shは、コードの一部が誤っており、実行すると意図した通りに動作しない。  
  どうやら`-b`と`-r`で、オプション使用時の挙動がテレコになっている様だ。  
  誤っている部分を修正しなさい  
  - 第一引数に、`-h`, `-b`, `-r`以外が指定された場合でも後続処理が実行されてしまっている様だ。  
  想定外の引数が指定された場合にスクリプトを終了させる処理を実装しなさい


