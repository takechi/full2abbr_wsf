・full2abbr.wsf
bib ファイルの雑誌名を正式名称から省略名称に置換する JScript

デフォルトでは AMS の公開している省略名リスト

http://www.ams.org/msnhtml/annser.csv

を自動で取得し、変換に利用する。
（利用しない場合は useAMS = false にする）


annser.csv と同じ形式（つまり、第 1 列が省略名称 "Abbrev" で、第 2 列が
正式名称 "Full Title"）の CSV を読み込ませて変換に利用することもできる。

例えば my.csv と aps.csv を読み込ませたい場合は

DBFilenames = ["my.csv", "aps.csv"];

とする。my.csv と aps.csv に同じ正式名称が登録されていた場合、先に書かれている
ファイル（上記の場合は my.csv）が適用される。
useAMS = true の場合、annser.csv が最後に適用される。




・aps.wsf
APS が公開している省略名リスト

https://authors.aps.org/STYLE/style_jabbr.html

を解析して annser.csv と同じ書式の csv ファイルに整形する JScript
