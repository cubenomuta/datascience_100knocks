# データサイエンス協会100本ノック記録
## Log
### 20230603(P-001~P-013)
  - [Kaggle日記](https://github.com/fkubota/kaggle-Cornell-Birdcall-Identification#readme)を参考にしながら初めてのGit Hubを書いてる
      - リポジトリの作り方とreadmeの書き方は何となくわかってきたが,ほかのフォルダの作り方とかテンプレの構造とが謎
      - 書き方テンプレは[このサイト](https://docs.github.com/ja/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#links)
      <br>
  - kaggleやsignateをやるにはまだまだ知識が足りないと痛感したので、まずはデータ分析、機械学習、統計の知識を身に着けることに
      - kaggleのコンペで実践する方がいいことは重々承知しているが、自分的には知識を先にインプットしてから実践していく方が性に合っているのでこうした
      - ある程度自身がついてきたらkaggleなどにも取り組んでいこうと思うので焦らず今はinputに集中する
      - 8月の夏休みにはコンペに参加するくらいのペースで頑張る
      - 今日は問1~13までをやった
      <br>
  - 以下に本日学んだ関数、引っかかった点を示す
      - 列名の変更 : rename  
            - #df_receipt = df_receipt.rename(columns = {'sales_ymd':'sales_data'})
      - query('customer_id == "CS018205000001"')  
            - C~の列を数字と勘違い → このように文字列の場合は"で囲う
      - query('customer_id == "CS018205000001" and amount >= 1000')  
            - クエリ条件に論理演算を加える場合それらを一つの'で囲う → 'a'and'b'のように分けるとうまくいかない
      - 文字列一致 : str.match, str.stratswith, str.endswith, str.contain  
            - df_store.query('store_cd.str.startswith("S14")').head(10)って感じで使う  
            - str.match(".*1$")は、.は任意の1文字、 *は0回以上の繰り返しを表す。 $は末尾の位置指定文字。 ^は先頭の位置指定文字。

 
  
### 20230604
  - 
