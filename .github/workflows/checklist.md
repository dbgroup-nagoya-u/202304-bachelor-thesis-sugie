# 論文執筆チェックリスト

## 進捗報告

- [ ] 進捗を共有している

## 章や節などの構成

- [ ] 段落が1つの項や節，文が1つの段落がない
- [ ] 研究の「背景」「動機」「目的」などに見出しをつけていない[参考](https://github.com/dbgroup-nagoya-u/202104-bachelor-thesis-hirano/pull/2#discussion_r801192646)
- [ ] 見出しつきの段落を多用していない
- [ ] タイトルで「~について」を使っていない
  - 概要について書きたいなら「～の概要」
- [ ] タイトルで「・」を使って複数列挙していない
- [ ] 節間や段落間の文量のバランスが適切である
- [ ] 「どこまでが既存研究でどこからが研究成果なのか」を明確にしている
  - 研究の新規性・優位性を明確にするため
- [ ] 関連研究を2章かまとめの手前に置き，「先行研究の概要」と「本研究の差異」を書いている [参考](https://github.com/dbgroup-nagoya-u/202004-bachelor-thesis-nishimura/pull/8#discussion_r571528882)

## 本文

- [ ] 1行1文になっている
  - レビューのしやすさと，1文が長くなりすぎていないか確認するため
- [ ] 1文目で節や段落の論旨を先に伝えている（リードセンテンス）
  - [パラグラフライティング](http://www.ams.eng.osaka-u.ac.jp/user/ishihara/?p=566)を意識する
- [ ] 先に定義や概要，後に具体的で細かい話をもってきている
  - 全体像を先に述べることで話を分かりやすくするため
- [ ] 一般的でない用語は説明してから使っている
- [ ] 用語を統一している
- [ ] 箇条書きによる説明は避けている
  - 図や表，段落での表現を検討する [参考](https://github.com/dbgroup-nagoya-u/202204-b4train-report-kuwamura/pull/4#issuecomment-1165160730)
  - 箇条書きにしたほうが見やすい場合は箇条書きを使う
- [ ] 箇条書きや表などで何かを列挙する際は末尾の表現を揃えている
- [ ] 手法の説明は現在形で書いている
- [ ] 実験環境・結果の説明など，明確に過去に行った事物の説明を過去形で書いている [参考](https://github.com/dbgroup-nagoya-u/202004-bachelor-thesis-nohara/pull/8#discussion_r574490580)
- [ ] 指示語は極力使用していない
  - 何を指しているのかが曖昧になりがちなため
- [ ] 「正式名称（略語）」の順で書いている
  - 例：Online Analytical Processing（OLAP）
- [ ] 日本語文中で英単語を使用する際は，先頭を大文字・小文字にするか文章全体で統一する
  - なお，小文字にする場合は一般的な英語文章のルール（固有名詞なら先頭は大文字，カンマの後には空白など）に従う
- [ ] 先行研究の参照は論文の著者名ないし手法名を使用している
  - 例：Qiら[7]は...，Bw木[11]では...
- [ ] 図や表，疑似コードを入れる場合は，示して終わりでなく説明を入れている
  - 特に疑似コードの説明はどの部分と対応しているかを明記する [参考](https://github.com/dbgroup-nagoya-u/202004-bachelor-thesis-nohara/pull/8#discussion_r572183483)
- [ ] スカラは小文字で，集合や行列は大文字で表している
- [ ] 疑似コード内に出てくる変数や関数は何を表しているか，何をしているかを説明している [参考](https://github.com/dbgroup-nagoya-u/202004-bachelor-thesis-nohara/pull/8#discussion_r573503682)
- [ ] 疑似コードの引数の説明はコメントではなく，直接書いている [参考](https://github.com/dbgroup-nagoya-u/202004-bachelor-thesis-suzuki/pull/4#discussion_r572023021)
- [ ] 疑似コードでの代入は "$\leftarrow$" [参考](https://github.com/dbgroup-nagoya-u/202204-bachelor-thesis-horisaki/pull/2#discussion_r1092668489)
  - "="は比較演算子
- [ ] 疑似コードにおける制御文（for, while, break, continue, etc...）は太字[参考](https://github.com/dbgroup-nagoya-u/202204-bachelor-thesis-horisaki/pull/4#discussion_r1096613955)
- [ ] 1000 ではなく 1,000と書いている
- [ ] 100,000以上は10万のように書いている
  - ただし，グラフの場合（後述）は指数を使う
- [ ] 数字~単位とする [参考](https://github.com/dbgroup-nagoya-u/202004-bachelor-thesis-nohara/pull/8#discussion_r574713763)
  - 数字と単位の間で改行されないようにするため
  - 必要に応じてsiunitxパッケージを使ってもいいかも
- [ ] 実験環境の記述をしている
  - [サーバスペック一覧はこちら](https://github.com/dbgroup-nagoya-u/dbgroup/wiki/%E3%82%B9%E3%83%9A%E3%83%83%E3%82%AF%E4%B8%80%E8%A6%A7)
  - OSとコンパイラのバージョンは各自で調べて記入する

## LaTeXの使い方

- [ ] 数式にはequationかalign環境を使用している
  - 数式の参照用に番号を振るため
- [ ] 段落に対して見出しをつけたい場合は\paragraph{}を使っている
- [ ] 図表の位置設定は[t]になっている
  - ただし，投稿先のジャーナルなどで体裁が定められている場合はそれに従う
  - また，1段組であればレイアウトに応じて[tb]としてもよい [参考](https://github.com/dbgroup-nagoya-u/202204-master-thesis-nishimura/pull/1#discussion_r1083592741)
- [ ] 図表は一番最初に参照した段落の後のスペースに置いている
  - 1段組の原稿では図表が「初めての参照以降」かつ「同じ節・項の範囲内」になるべく表示されるように調整する
    - 複数の図表が同ページ内で上下に散らばるのは嫌なので，あくまでなるべく
  - 2段組の文章で1段組の図表（i.e., `begin{figure*}...end{figure*}`）を使用する場合は，適切な位置に出力されるよう挿入位置を調整する
- [ ] 図表には\labelを貼って，\Sec,\Subsec,\Fig,\Tabなどの[定義済みマクロ](https://github.com/dbgroup-nagoya-u/template-latex/blob/096d98c95f6ef4c16db659fdc72198a1722e2a2b/src/my_command_definitions.sty)で参照している [参考](https://github.com/dbgroup-nagoya-u/202004-ipsj2021-nohara/pull/7#discussion_r550384629)
  - 図のラベルは fig:figname，表のラベルは tab:tabname とすると区別が楽
- [ ] タイトルをキリが良いところで改行している

## 参考文献（*.bib）

- [ ] 発行している学会のページ（IEEEならXplore，ACMならDigital Library）から得られるものをベースに作成している
- [ ] 有名所の会議や論文誌を参照するときは略称を使う（略称はHPを確認）[参考](https://github.com/dbgroup-nagoya-u/202204-bachelor-thesis-kuwamura/pull/31#discussion_r1104009975)
- [ ] カテゴリがinproceedingsの論文（i.e., 国際会議論文）はProc. xxxとして略記している [参考](https://github.com/dbgroup-nagoya-u/202004-ipsj2021-nishimura/pull/5#discussion_r551708006)

## 図

- [ ] 図の作成にはPowerPointを使用している
- [ ] スライドの横幅を段組みの横幅に合わせている
  - IPSJ原稿のようなA4の2段組の場合横80mm
  - 卒業論文など1段組は120～150㎜
- [ ] 図の文字色を黒に変えている
  - パワポのグラフはなぜかデフォルトで文字色は灰色
- [ ] 図中の文字サイズをキャプションの文字サイズとおおよそ揃えるか，少しだけ大きくする
  - PSJ原稿のようなA4の2段組の場合8ptくらい
  - 卒業論文など1段組は10～11pt
- [ ] 英数字のフォントが「Cambria Math」
  - 論文の英数字のフォントとこれが一番似ていて，かつオープン利用可能
- [ ] 日本語のフォントが本文と同じ明朝体（游明朝とか）
- [ ] スライド上下の余白はギリギリまで削っている
  - LaTeX側で自動で余白が挿入されるため
- [ ] 作成した図はPDFでエクスポートしている
  - 拡大しても画質が落ちないため
- [ ] キャプションを具体的に書いている
  - キャプションだけで何の図が分かるように
- [ ] 複数の図を入れるときはサブのキャプションを追加して参照しやすくしている
  - 自前で入れるか，別々の図として作成してsubcaptionパッケージを使うか

### グラフに関する事項

- [ ] 論文中で使うグラフは本リポジトリ内のテンプレート（[これとか](https://github.com/dbgroup-nagoya-u/template-latex/blob/4a4c5887d4f268e466e2e6e051bddeb54b2d4020/src/figures/graph-grouped_methods.pptx)）を改変したものを利用している
- [ ] Excel側でグラフタイトルをつけていない
  - LaTeX側でキャプションをつける
- [ ] 折れ線グラフを散布図スタイルで作っている
  - 対数スケールで表示したり，2の倍数でパラメータを変えたりする際に正確にプロットできる
- [ ] 罫線はなるべく減らし，代わりに目盛りを入れている
- [ ] グラフの線の分類を色だけに頼らず，破線や点線を使っている
  - 色弱の人への配慮
- [ ] 桁が大きい場合，指数を使って表現している