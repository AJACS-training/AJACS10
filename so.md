[[AJACS10]]

        --
目次

#contents
        --
# Genome AnnotationとKazusa Annotation（かずさDNA研・○岡本忍、中尾光輝、藤澤貴智、中村保一） [#vc393b61]

## 【実習1】ゲノムアノテーションの検索例その１：NCBI Entrezで光合成系２のタンパク質のアノテーション（注釈）を眺めてみましょう [#je492cae]

- NCBI Entrezのページ
- http://www.ncbi.nlm.nih.gov/gquery/

+1. "Photosystem II"で検索してみる。少し多すぎる？
+2. "Photosystem II AND Synechocystis AND PsbA2"で絞り込んで検索してみる。
+3. Proteinの検索結果は何件？　→　http://www.ncbi.nlm.nih.gov/sites/entrez?db=protein&cmd=search&term=Photosystem%20II%20AND%20Synechocystis%20AND%20PsbA2
+4. Proteinのエントリー BAA16586 を眺めてみよう。→　http://www.ncbi.nlm.nih.gov/protein/1651658?ordinalpos=1&itool=EntrezSystem2.PEntrez.Sequence.Sequence_ResultsPanel.Sequence_RVDocSum
+5. BAA16586のDEFINITIONと書かれた行に注目してみよう。


## 【実習2】ゲノムアノテーションの検索例その２：UniProtKBで光合成系２のタンパク質のアノテーション（注釈）を眺めてみましょう [#n598b61d]

- UniProtKBのページ
- http://www.uniprot.org/help/uniprotkb

+1. 左側のプルダウンメニュー「Search in」を「Protein Knowledgebase」にする。
+2. 検索窓「 Query」の部分に"Photosystem II"と入力して検索してみる。→　http://www.uniprot.org/uniprot/?query=Photosystem+II&sort=score
+3. 検索窓「 Query」の部分に"Photosystem II AND Synechocystis AND PsbA2"と入力して検索してみる。→　http://www.uniprot.org/uniprot/?query=Photosystem+II+AND+Synechocystis+AND+PsbA2&sort=score
+4. エントリー P16033を眺めてみよう　→　 http://www.uniprot.org/uniprot/P16033
+5. P16033の更新履歴を見てみよう。→　http://www.uniprot.org/uniprot/P16033?version=*
+6. version 74と80を比較してみよう。→　http://www.uniprot.org/uniprot/P16033?version=74&version=80

- イミラー問題  →　http://www.uniprot.org/uniprot/?query=imilar&sort=score



## 【実習3】KazusaAnnotationの利用例 [#jfb52198]
+1. http://a.kazusa.or.jp/ を開いてみましょう [[（画像）>http://MotDB.DBCLS.jp/?plugin=attach&pcmd=open&file=%A5%D4%A5%AF%A5%C1%A5%E3%201.png&refer=AJACS5%2Fyn]]
+2. 酸素発生型光合成細菌の'''Synechocystis'''の光合成系IIの遺伝子psbAのアノテーションを検索しましょう。右上の検索窓に「Synechocystis psbA」と入れて「検索」を押します。
+3. このように検索結果が表示されます→ http://a.kazusa.or.jp/annotation?q=Synechocystis+psbA
+4. 検索結果のなかの遺伝子 slr1311 の赤い字でしめされた「1520 annotations」をクリックするとslr1311遺伝子につけたアノテーション（ブックマーク）が一覧されます。→ http://a.kazusa.or.jp/annotation/show?uri=http%3A%2F%2Fbacteria.kazusa.or.jp%2Fcyanobase%2FSynechocystis%2Fcgi-bin%2Forfinfo.cgi%3Ftitle%3DChr%26name%3Dslr1311%26iden%3D1
+5. Pubmed ID: のなかから、9154987 をクリックすると、論文の情報が表示されます。そこからPubmedに行くこともできます。→ http://a.kazusa.or.jp/tags/show?name=pmid%3A9154987
+6. 論文情報の下部分「アノテーション数:50」は、この論文PubMed ID 9154987にGene Indexingが50個つけられてることを表している。
数字の「50」の部分をクリック。slr1311以外に、sll0851, slr0906, sll0849, slr1181など8個の遺伝子にも言及してることがわかる。
+7.論文情報の下部分「Gene Indexing View」をクリックすると、MeSH Termが見られる。また、文献書式（Title, Abstract, Introduction...）のどこに、どの遺伝子が記述されているのかが参照できる。タイトルやアブストラクト、ディスカッションに出てる遺伝子は、この論文のメインテーマであると類推できる。→　http://a.kazusa.or.jp/tag/geneindex/pmid:9154987

- かずさDNA研究所が提供している、シアノバクテリア（光合成細菌）、根粒菌のデータベース →　http://genome.kazusa.or.jp/
    - CyanoBase（光合成細菌）→ http://genome.kazusa.or.jp/cyanobase
- CyanoBaseで光合成系２遺伝子 slr1331をみてみよう。→ http://genome.kazusa.or.jp/cyanobase/Synechocystis/genes/slr1311
    - CyanoBaseのslr1331のページからKazusaAnnoationを参照する。上から５段目のGene Annotationのところ


## 【応用編】論文と遺伝子の関係性を俯瞰する：[[ Cytoscape >http://www.cytoscape.org/ ]] でみる KazusaAnnotation/Gene Indexing [#r9c54cb2]
- http://charles.kazusa.or.jp/~so/ajacs10/syn_allgenes_ajacs5.cys：Cytoscapeで開くとレイアウトされた状態で見ることが出来ます。検索等も可能。
- http://charles.kazusa.or.jp/~so/ajacs10/syn_allgenes_cyt.txt：syn_allgenes_ajacs5.cysを描画するための遺伝子-文献(言及頻度）の二項関係データ、Synechocystis全遺伝子
- http://charles.kazusa.or.jp/~so/ajacs10/syn_path00195_cyt.txt：syn_allgenes_ajacs5.cysを描画するための遺伝子-文献(言及頻度）の二項関係データ、Synechocystis光合成関連遺伝子


## 【参考1】Biocuratorについて [#vfc3f89e]
- 生物に関する様々な情報を整理、統合、付与しゲノム情報の価値を高めるスペシャリスト
- 学会サイト →　 http://www.biocurator.org/
## 【参考2】集合知的なもののパワー [#je36221e]
- 日本全国の鉄道の駅のデーターベース　→　http://ja.wikipedia.org/wiki/日本の鉄道駅一覧
- ポストマップ：ポストをひたすらマッピング →　 http://postmap.org/
## 【参考3】OpenID について [#v1674e12]
- OpenIDを使うと、KazusaAnnotationにあなた自身がブックマークを登録することができます。
- こちらをご覧ください。統合TV「統合DBを使い倒すためにOpenIDを取得する」http://togotv.dbcls.jp/20080507.html
- [[openid.dbcls.jp>http://openid.dbcls.jp]]
 DBCLS OpenID サービス は、DBCLS が提供する OpenID 認証サービスです。
 統合データベースプロジェクトをはじめとした OpenID に対応しているサイトについて、
 ひとつのアカウントでアクセスすることができます。
 使いかたはヘルプを御覧下さい。統合TVによる使いかた紹介
 (統合DBを使い倒すためにOpenIDを取得する)も併せて御覧下さい。
- ご自身のメイルを受け取ることのできる環境で、OpenIDを取得してください
- 統合DBサービスの標準認証サービスです。Kazusa Annotation Suite以外に http://lifesciencedb.jp/ などで活用できます。


        --

##  [[KazusaAnnotation>http://a.kazusa.or.jp/]] 【http://a.kazusa.or.jp】 [#r23f2f76]
- ソーシャルブックマークによるゲノムアノテーション蓄積／改善／統合サイト。
- 66,255 エントリ 220,993 アノテーション 15,988 タグ (2009年5月15日0時現在)


## [[KazusaNavigation>http://navi.kazusa.or.jp/]] 【http://navi.kazusa.or.jp】 [#l1d43b54]
- コミュニティの形成や活性化をめざしたサイト
- ソーシャルネットワークサービス (SNS)の Elgg ( http://elgg.org ) を改変して用いています

###  KazusaNavigationの利用例 [#u736341d]
+1. http://navi.kazusa.or.jp を開き [[（画像）>http://MotDB.DBCLS.jp/?plugin=attach&pcmd=open&file=%A5%D4%A5%AF%A5%C1%A5%E3%208.png&refer=AJACS5%2Fyn]]
+2. 右上の検索窓の下にある「一覧」をクリック＞プロジェクトとユーザの一覧が表示されます [[（画像）>http://MotDB.DBCLS.jp/?plugin=attach&pcmd=open&file=%A5%D4%A5%AF%A5%C1%A5%E3%209.png&refer=AJACS5%2Fyn]]
+3. あるいは http://www.google.co.jp で「KazusaNavigation 植物研究関連イヴェント」「KazusaNavigation 植物研究者人材募集」で 検索
+4. 「植物研究関連イヴェント」を閲覧する [[（画像）>http://MotDB.DBCLS.jp/?plugin=attach&pcmd=open&file=%A5%D4%A5%AF%A5%C1%A5%E3%2010.png&refer=AJACS5%2Fyn]] [[（画像）>http://MotDB.DBCLS.jp/?plugin=attach&pcmd=open&file=%A5%D4%A5%AF%A5%C1%A5%E3%2011.png&refer=AJACS5%2Fyn]]
+5. 「植物研究者人材募集」も同様に閲覧してみましょう。

- &ref(rss.png); RSSをブラウザに登録しておけば、毎回見に来る必要はありません。新着が報告されます
    -RSSとは？ see → http://ja.wikipedia.org/wiki/RSS

- OpenIDを取得すると、プロジェクト（コミュニティ）を作るなど、コンテンツを作成し共有することができます。

        --

## [[KazusaWiki>http://wiki.kazusa.or.jp/]] 【http://wiki.kazusa.or.jp】 [#q9009138]
Wikipediaと同じ、Mediawikiというプログラムを利用した情報とりまとめ用サイト

###  KazusaWikiの利用例 [#j4affcf3]
+1. http://wiki.kazusa.or.jp を開く [[（画像）>http://MotDB.DBCLS.jp/?plugin=attach&pcmd=open&file=%A5%D4%A5%AF%A5%C1%A5%E3%2012.png&refer=AJACS5%2Fyn]]
+2. あるいは、http://www.google.co.jp で「KazusaWiki トマト」で検索し [[（画像）>http://MotDB.DBCLS.jp/?plugin=attach&pcmd=open&file=%A5%D4%A5%AF%A5%C1%A5%E3%2013.png&refer=AJACS5%2Fyn]]
+3. トマト研究会 JSOL（ http://wiki.kazusa.or.jp/JSOL ）のコンテンツを開いてみる [[（画像）>http://MotDB.DBCLS.jp/?plugin=attach&pcmd=open&file=%A5%D4%A5%AF%A5%C1%A5%E3%2014.png&refer=AJACS5%2Fyn]]

- OpenIDを取得すると、Wikiのコンテンツを作成し共有することができます。研究会の情報共有などにどうぞ。

        --

[[AJACS10]]
