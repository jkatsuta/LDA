# LDA

トピックモデル（LDA）がテーマのブログのためのコード集です。  
ブログURL: http://recruit.gmo.jp/engineer/jisedai/blog/topic-model/


もし実際に動かしたい場合は、  
gensim (https://radimrehurek.com/gensim/),  
Meacab (http://taku910.github.io/mecab/)  
が必要です。

一応、今回使ったデータの準備方法(ana_wiki1.ipynb用の前処理)も紹介しておきます。

1. 日本語Wikipediaのデータ取得  
https://dumps.wikimedia.org/jawiki/latest/jawiki-latest-pages-articles.xml.bz2

2. bz2を解凍後、txt -> xml化  
$ wp2txt --input_file ./jawiki-latest-pages-articles.xml  
(入ってなければ、$ gem install wp2txt)

3. ./jawiki_data/というdirectoryをつくり、txt化したファイル群を移動
