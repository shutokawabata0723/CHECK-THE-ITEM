# CHECK-THE-ITEM
This program automatically check items you want and let you know when condition change or price reduction happen.
<br>
お気に入りに登録してある商品の在庫状況と価格を常に監視します．
<br>
在庫状況と価格に変化があればお知らせします．

# Purpose
To monitor items you want and if the item exists or changes its price lower than before, 
notify by E-mail and noticeing function on Macbook.<br>
So, you can accept the notice soon while outing and get item you want.


お気に入りに登録したの商品の在庫状況と価格を常に監視し，在庫が復活するか価格が下がると同時にお知らせします．
<br>
EメールとMacbookの通知機能を使ってお知らせを行います．
<br>
人気がある商品の在庫・価格を自動で監視してくれるので，携帯を気にする必要がなくなります．
<br>
外出先でも通知が来るので安心です．
<br>
また，同じカテゴリ内でどの店舗が一番安く売っているのかがわかるので，非常に効率よく買い物ができます．

# Contents
## item_list.csv
input file, URL of the item you want, ideal price you want to be noticed, category
<br>
入力ファイルです．ここに，”欲しい商品のURL”，”通知を受ける条件価格”，”商品のカテゴリ” を入力してください．


## In_stock.csv
output file, if the item is in stock, price, real price including tax and point, the lowest price in same category, URL are saved as a list.
<br>
出力ファイルです．在庫のある商品と現時点での同じカテゴリ内の最安値，その店舗を表示します．
メールにも同じ内容の通知が来ます．



## zaiko.pl
program code, monitor the item's stock condition and price.<br>
Scrape HTML and extract name of item, condition of the item and price.<br>
further more, find the lowest price and store in same category.

# How to use
1. Prepare input file.<br> 
2. change here as your sending e-mail address -->https://github.com/shutokawabata0723/CHECK-THE-ITEM/blob/master/zaiko.pl#L124 <br> 
3. change here as your receiving e-mail address -->https://github.com/shutokawabata0723/CHECK-THE-ITEM/blob/master/zaiko.pl#L152 <br>
4. excute zaiko.pl<br>

<img src="https://github.com/shutokawabata0723/CHECK-THE-ITEM/blob/master/zaiko-screen.png" width="700px"><br>

# Caution
The program probably stop if URL of the item does not exist or style of the HTML changed.<br>



# Licence
CopyRight (c) 2018 Shuto Kawabata

Released under the MIT licence

https://opensource.org/licenses/MIT

# Author
Shuto Kawabata


