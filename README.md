# oer-infrastructure
This is a repository of considering about a system of open educational resources (OER) infrastructure.
# English

# 日本語/Japanese
## 背景
知識の重要性が飛躍的に向上した知識基盤社会の中にあると言われる昨今、属性関係なくいつでも質の高い教育を受けられる生涯学習社会の実現の重要性は日に日に高まっている。
その中でオープンエデュケーションによる教育の開放・蓄積・改善が求められ、その代表的なものにOpen Educational Resources (OER)を利用したOpen Educational Practices (OEP)がある。だが、それに必要な持続可能なOERインフラは未だに未整備のため、OEPは実現には程遠い現状である。
よって、このリポジトリでは持続可能なOERインフラの構想、設計をついて扱う。

https://www.mext.go.jp/b_menu/shingi/chukyo/chukyo0/toushin/attach/1397420.htm
https://www.mext.go.jp/content/20210720-mxt_soseisk01-000016965_2-3.pdf
https://www.jstage.jst.go.jp/article/johokanri/59/1/59_3/_html/-char/ja
https://en.wikipedia.org/wiki/Open_educational_resources
https://ict.axies.jp/_media/sites/11/2023/08/2020_axies_ict_survey_result.pdf

## 考慮すべきポイント
### 利点・欠点
構築の際、これらの利点・欠点をうまく制御する必要がある。
https://en.wikipedia.org/wiki/Open_educational_resources#Advantages_and_disadvantages

### 5R
閉鎖的な教材と比べたOERの重要な特徴として5R(保持:Retain、再利用:reuse、改訂:revise、リミックス:remix、再配布:redistribute)の積極的支持がある。よって、それらが十分に可能なインフラでなくてはならないが、それらはどの様な形で持続可能なシステムとできるかは明らかでない。

この論文が詳しい。
Heck, Tamara et al. “Designing Open Informational Ecosystems on the Concept of Open Educational Resources.” Open Education Studies 2 (2020): 252 - 264.

https://papertohtml.org/paper?id=09c723652dd80c64ec404b45cf1b4a29a6e52d08

部分的には以下のような機能が必要となる。
- 保持
  - OER のダウンロード
- 再利用
  - 適切なメタデータ標準の使用、検索インターフェース、検索結果のランキング
- 改訂
  - A: OER 用にダウンロードしてアップロードするか、B: Web エディターまたはコメントオプションを使用する
- リミックス
  - A: OER 用にダウンロードしてアップロードするか、B: Web エディターまたはコメントオプションを使用する
- 再配布
  - 新しい OER をアップロードするか、教育メタデータ標準などに新しい参照を追加する
 
### 学習オブジェクト
また、再利用には教材が再利用しやすい粒度である必要がある。その粒度の教材を学習オブジェクトと呼ぶ。

https://en.wikipedia.org/wiki/Learning_object

### コネクティビティビズム

### 互換性
SCORM、xAPI、cmi5、AICC標準により、Moodleなどの他のLMSで利用できるようにする。
https://en.wikipedia.org/wiki/Sharable_Content_Object_Reference_Model
SCORM、xAPI、cmi5、AICC標準

### 公共財化
5Rは教材に非排除性(誰でも使える)と非競合性(少数に利用を占領されない)を持たせることで公共財化することであると考えられる。そのため、公共財特有の特徴を設計時に考慮する必要がある。具体的にはフリーライダー問題や政府の関与などである。

https://en.wikipedia.org/wiki/Public_good_(economics)
https://en.wikipedia.org/wiki/Free-rider_problem

### Wikipediaとの違い
Wikipediaは辞書であり、中立的で高い真実性である記述を追及している。だが、OERはそれらに加えて、高い教育効果やノウハウなどの意見の一致を得ることが難しいものの提供を行う。そして最終的は、学習効果の測定やノウハウを巡る議論などを通して、それらを辞書に取り込めるほどの知識として確立していくことを目指す。




### 権威への対応
誰でも自分の作ったものが酷評され、権威が損なわれるのは苦しい。特に個人が特定されるものであればなおさらである。そのため、積極的な参加を促すには、教材が高評価であった場合のみ作成者を公表するなどが必要となる。また、MOOCへの教育機関の関与の背景には、権威向上の意味がある。よって、OER提供を行うことで、そのような個人、団体の権威をデメリット無く、向上させる仕組みが必要がある。

### 資金調達
このようなインフラを開発、運用するにはある程度の資金が必要となる。持続可能なビジネスモデルを構築しなければならない。
フリーミアム、無料トライアル + 有料サブスクリプション、広告 + 広告なしのサブスクリプション、学区・大学の管理者・その他の意思決定者への売り込み、エンタープライズ/B2Bセールス、政府・教育機関・非営利団体とのパートナーシップ、企業スポンサー、採用分野への進出などがある。だが、最終的なビジネスモデルの決定は、実際のユーザーでの仮説検証を繰り返しながら、柔軟に決めていくのが望ましい。

https://www.mindk.com/blog/edtech-startup-business-model/
https://en.wikipedia.org/wiki/Open_educational_practices#Strategies_and_recommendations

### 法律と政策
大きな問題として著作権処理がある。だが授業目的公衆送信補償金制度により、月数百円程度を支払うことで著作物の含まれる教材を利用できる可能性がある。

https://sartras.or.jp/seido/

### 官民連携
社会的な重要性が高いため官民連携を図ることも視野に入れる。

### ステークホルダーの構築
教材作成者と教材利用者だけでなく、教育機関や政府機関、教師、研究者、著作権専門家、非営利団体、教育産業などの様々なステークホルダーと利害調整を行う必要がある。

### 品質評価
教材の発見可能性、インフラの信頼性には教材の品質を高い精度で評価する仕組みが必要である。これには査読のような方法が考えられているが、持続可能性は低いため新たな方法が必要である。

### 新しい教育への順応
OEPは教育をOERを使って革新していくことを目的としている。だが、急激な発展にステークホルダーを順応させるのは困難で、なだらかな発展と十分な補助を基にステークホルダーが確実に新しい教育へ順応が出来るように設計する必要がある。よって、最初から完全な革新を断行するのではなく、ステークホルダーの慣れ親しんだツールや方法を徐々に革新していく戦略が望ましい。

## 戦略
オープンエデュケーションには

ステークホルダー
ユーザーは大きく教材作成者と教材利用者に分けられる。
OERの利用を促進するには質の高いOERを充実させる必要があり、それには優秀な教材作成者の継続的参加が欠かせない。よって、まずはそれを実現する施策を行う。
OERの大きな利点は教材の


