# IAB_Citation
Yuki Okada  
Last Update: 2024-11-27
- [purpose](#purpose)
- [usage](#usage)
- [update](#update)
- [references](#references)

----------

## purpose
IAB_Citationは，IABの引用形式に則したCSL(Citation Style Language)ファイルを格納したディレクトリです．

CSLとは文献の引用形式をXMLで記述したものであり，文献管理ソフト(Mendeley,Paperpile,Zoteroなど)で読み込んで使用します．

これにより，TPでの引用形式に関する添削を軽減することを目的としています．

----------

## usage
### CSLファイルの読み込み
CSLファイルの読み込みについては，各ソフトウェアによって異なるので調べてみてください．

- [Mendeley](https://www.umi-mori.jp/article/science/mendeley_tutorial)
- [Mendeley Cite](https://psycho.hes.kyushu-u.ac.jp/mendeley-csl-editor/)
- [Paperpile](https://paperpile.com/h/guide-google-docs/)
- [Zotero](https://www.zotero.org/support/preferences/cite)

URLを使ってインポートする場合は，こちらを使用して下さい．
https://raw.githubusercontent.com/t5a57l/IAB_Citation/refs/heads/main/NLM_IABver_ver1.1.csl

### 雑誌名の省略形
雑誌名の省略形を使用したい場合は，文献管理ソフト側で設定して下さい．

### 引用が正しくできない場合は？
文献管理ソフトに文献情報が正しく登録されているか確認してください．

雑誌論文の場合は，**著者名，論文名，雑誌名，出版年，巻，号，ページ数**の情報が必要です．

----------

## update
### ver1.0

IABの基本的な引用形式を実装した．

- 本文、表、図版の説明文における参考文献をブラケット`[]`で囲んだアラビア数字によって示す
- 冒頭の６名までの著者を列挙し、著者が７名以上いる場合は、 et al. 表記で省略する
- 出版日は年のみとし、月と日付は含めない
- 雑誌論文の場合はURLや引用した年月日，`[Internet]`などを表記しない(文献管理ソフト側での追加設定は不要)

### ver1.1

cslファイル内のIDを固有のものに変更．

`<id>http://www.zotero.org/styles/taylor-and-francis-national-library-of-medicine</id>`
→`<id>http://www.zotero.org/styles/taylor-and-francis-national-library-of-medicine/iab-nlm</id>`

### citation_for_research_plan.csl

研究計画やポスター用の簡潔な引用形式

* 著者が2名以上の場合は筆頭著者のみを表示し「et al.」を追加（例：`Sasagawa, S., et al.`）
* 出版年を括弧付きで表示（例：`(2013)`）
* 雑誌名をイタリック体で表示
* 号番号（issue）を括弧付きで表示し、巻とページを`巻(号)`: ページの形式で表示（例：`152(3): 945–956`）
* 参考文献リストの形式：`[1] Sasagawa, S., et al. (2013) Cell, 152(3): 945–956.`

----------

## references
- [先端生命研 - Submission Guidelines](https://sites.google.com/keio.jp/sfc-bio/guide/term-papar/submission-guidelines)
- [NLM Examples - National Library of Medicine Citation Style - Life Chiropractic College West Library at Life Chiropractic College West](https://libguides.lifewest.edu/citation-format/NLM-examples)
- [CSL 1.0.2 Specification — Citation Style Language 1.0.1-dev documentation](https://docs.citationstyles.org/en/stable/specification.html#namespacing)
