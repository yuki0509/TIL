### branchとmergeについて

branchとは => 並行して複数機能を開発するためにあるのがブランチ。ブランチを分けることで他の人が加えた修正が自分の開発に影響しないというメリットがある。
よく見るHEADについて => これは現在のブランチを刺す

branchコマンド<br>
ブランチ表示 git branch  
新規作成 git branch ブランチ名  
ブランチ切り替え git checkout ブランチ名, git checkout -b ブランチ名

mergeとは => mergeとはほかの人の変更内容を自分が現在作業しているブランチに取り込むこと。

mergeコマンド<br>
git merge ブランチ名  
git merge リモート名/ブランチ名  

<strong>mergeには3種類ある！！</strong>
1.早送りになるマージ  
枝分かれしてなくブランチがブランチのポインタを前に進めるだけ。

2.基本的なマージ  
作業中のブランチをベースにしてマージしたブランチのファイルの内容を加える。新しくマージコミットが作られる

3.コンフリクト  
コンフリクトとはファイル同士の衝突のこと。マージしたときにファイルの同じ行に違うことが記載されてたら、コンフリクトがおこる。  
違う人が同じファイルを扱わないなどの工夫が必要。  

#### ブランチの変更・削除  
変更 => git branch -m ブランチ名  
削除 => git branch -d ブランチ名, git branch -D ブランチ名 -Dはマージされてない変更が残っていても強制的に削除される。  

***リモートブランチとは***  
リモートリポジトリ内のブランチ。git fetch でブランチをローカルPCにもってくることができる。
<pre>remote/origin/master</pre>などのように表される。


