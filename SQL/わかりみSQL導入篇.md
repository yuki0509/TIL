# データベースとは  

- データベースとは、様々なデータの検索や登録や変更や削除ができるシステムのこと。

### リレーショナルデータベース  
データベースの種類の一種で、現実のシステムで一番よく使われている種類のデータベース。データを種類ごとにテーブルの形で保持しておき、
必要に応じてテーブルを連結したり、加工したりするデータベース。

### SQL
RDBからデータを検索したり、加工したりする言語。

### データベースの特徴  

1.データとロジックの分離  
エクセルはデータとロジックが一つになっているため、一つのことしか実行できない。
しかし、DBはロジックが分離しているため、一つの同じテーブルでもロジックを分ければ違う処理ができる。（平均点や合計点など。）

2.データを柔軟に組み合わせられる
RDBはデータの種類ごとに細かくテーブルを分けることができる。そして必要に応じて、テーブル同士を結合してデータを処理することができる。**結合された
データを分離するよりも、分離されたデータを結合する方がずっと簡単だ。**

3.データを整合性を保つ  
エクセルは、他の箇所で使用中のデータを消せてしまい、データの整合性を保てない。しかし、RDBでは登録済みのデータしか使用することができず、尚且つ
**他で使用中のデータは誤って消せないようにしている。**

4.データの修正漏れを防ぐ  
エクセルはデータが複数の箇所に保存されており、修正を加えるときは全ての箇所を変更しないといけない。一方、RDBはデータは一箇所に保存して、テーブルを
結合して利用するため、データを修正したいときは一箇所だけ修正すればいい。  

5.同時変更による競合の考慮   
ファイルの修正が同時に行われると、エクセルでは混乱してしまうが、RDBでは**トランザクションが起こり、整合性が取れない場合はキャンセルされる。**

6.大量のデータ保存  
RDBの方、何十おくものデータを保存でき、別のサーバーを用意すればさらにデータを保存できる。  

# テーブルの構造について  
テーブルは、行と列から構成されます。行を識別するのは、「値」だけど列を識別するのは値でなく「名前」（列名）である。



