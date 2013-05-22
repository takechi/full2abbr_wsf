full2abbr.wsf
-------------

bib ファイルの雑誌名を正式名称から省略名称に置換する JScript

デフォルトでは JabRef の公開している省略名リスト

http://jabref.sourceforge.net/journals/journal_abbreviations_general.txt

および AMS の公開している省略名リスト

http://www.ams.org/msnhtml/annser.csv

を自動で取得し、変換に利用する。
（利用しない場合は useJabRefDB または useAMSDB を false にする）


annser.csv と同じ形式（つまり、第 1 列が省略名称 "Abbrev"、第 2 列が
正式名称 "Full Title" で、それぞれダブルクォーテーションで囲む）の CSV を
準備すれば、それを変換に利用することもできる。

例えば my1.csv と my2.csv を読み込ませたい場合は、それらを full2abbr.wsf と
同じフォルダに置き、

DBFilenames = ["my1.csv", "my2.csv"];

とする。my1.csv と my2.csv に同じ正式名称が登録されていた場合、先に書かれている
ファイル（上記の場合は my1.csv）が利用される。




aps.wsf
-------

APS の公開している省略名リスト

https://authors.aps.org/STYLE/style_jabbr.html

を解析して annser.csv と同じ書式の csv ファイルに整形する JScript

JabRef の省略名リストにほぼ同じ情報があるので、ほぼ必要ない。
