# Open Discovery Design

**AIと作っていたら、考え方や開発の仕組みまで育ってきた。**

Open Discovery Design（ODD）は、最初から完成したFrameworkとして設計されたものではありません。

IdeasというProductを、人とAIで実際に作りながら、

- 人とAIはどう一緒に考えられるか
- AIが意味形成へ関わるとき、何を守るべきか
- ObservationをどうProductへ戻すか
- AIをTeamとして使うとき、RoleやContextをどう分けるか
- 開発中に生まれたKnowledgeをどう残し、引き継ぎ、公開するか

といったQuestionに向き合う中で、少しずつ形になってきたWorking Knowledgeです。

> **思想を先に完成させてProductへ適用したというより、Productを作っていたら、思想・設計・チーム・運用が少しずつ析出してきた。**

You probably don't need most of this.
I do.
Take what you need.


## ひとつのQuestionから始まった

Ideasの初期には、こんなQuestionがありました。

> **問いになる前から、人とAIは一緒に探索できるだろうか。**

人は、最初から明確なQuestionを持っているとは限りません。「なんとなく気になる」「少し引っかかる」「まだ言葉にはできない」。そんなAttentionからAIと一緒に少し考えることはできるだろうか。Ideasは、そのQuestionをProductとして試しています。

そのProductを作る過程で、Product Designだけでは収まらないQuestionが増えていきました。それが現在のODDにつながっています。

→ [ODDがIdeasからどう生まれたか](./cases/ideas-origin.md)

## ODDとは何か

短く言えば、ODDは現在、

> **実際のAI-native Product Developmentから生まれた、公開中のWorking Knowledge**

として扱っています。

完成したMethodologyでも、Universalな正解でもありません。Concept、Practice、Observation、Case、Open Question、Mapを、現在のKnowledge Strengthをできるだけ保ったまま公開しています。

### 用語について

ODDの用語の多くは、理論を構築するために先に作ったものではありません。実際の探索や開発中に、**「これとこれは区別したい」**となったときに置かれたWorking LabelやLocal Shorthandです。

名前が付いていても、それだけでCore ConceptやPrincipleという意味ではありません。覚える必要もありません。今のProblemを扱うために必要なものだけ使ってください。

> **Named ≠ Fundamental.**  
> **Useful label ≠ Universal theory.**

## まず全部読む必要はありません

ODDを理解するために、最初から全部読む必要はありません。今の興味から入ってください。

- 説明より、まず1つ試したい → [Try one ODD failure](./try/README.md)
- 「ODDって何？」 → [Sitemap](./maps/sitemap.md)
- ODDと近い既存Conceptを知りたい → [Related Concepts](./related-concepts/README.md)
- 人とAIがどう一緒に考えるか → [Co-Explorer](./concepts/co-explorer.md)
- AIが意味へ影響することが気になる → [Meaning Authority](./concepts/meaning-authority.md)
- AIでProduct Developmentする方法に興味がある → [AI Product Team](./practices/ai-product-team.md)
- 理論より、実際に起きたことを見たい → [User0 Selected Observations](./observations/user0/selected-observations.md)
- Knowledgeがどう更新されるか → [Observation to Design](./practices/observation-to-design.md)
- AIにこのRepositoryを読ませたい → [AI Reading Guide](./ai-reading-guide/README.md)
- ODDを自分のProjectへ持っていきたい → [Forking Guide](./forking/README.md)

## まず、1つだけ試してみる

ODDを理解してから使う必要はありません。

Ideas / ODDの開発中には、たとえばこんなFailureが実際に起きました。

- AIが質問しすぎて、探索がインタビューになった。
- 作ったAIにそのままReviewさせたら、作者側のContextに引っ張られた。
- 良いと思ったRuleを守ったのに、実際の体験が悪くなった。
- 過去には妥当だった判断を、AIが現在にも適用し続けた。
- 「なぜそう決めたか」の空白を、AIが綺麗なStoryで補完した。

似たFailureがあれば、ODD全体ではなく、そのケースだけForkして試せます。

→ [Try one ODD failure](./try/README.md)

> **Try one failure. Fork only what you need.**

### たとえば、Fresh Reviewを1回だけ試す

同じAIに「作る」と「レビューする」を続けて頼むと、制作中の意図や判断Contextに引っ張られ、レビューが作者側へ寄ることがありました。

最初に試せるのは、**制作とレビューのContextを分ける**ことです。

**Minimum Fork:** [`try/fresh-review/`](./try/fresh-review/)

制作Sessionとは別Sessionを作り、Reviewerには制作過程の全Contextを原則渡しません。

ただし、Fresh Reviewは「情報を与えないレビュー」ではありません。レビュー対象の**最新成果物・最新ドキュメント・評価に必要な前提**は渡します。

> **Fresh context does not mean missing context.**

まず1回、いつもの制作Sessionとは別のSessionでレビューして、論点の出方が変わるか観察してみてください。

継続的にRoleを分けて使いたくなったら、[`try/ai-product-team/`](./try/ai-product-team/) へ広げられます。背景や限界を知りたくなったら、[AI Product Team](./practices/ai-product-team.md) と [Handoff](./practices/handoff.md) へ進んでください。

## Human-friendly entrances. AI-friendly depth.

Public ODDでは、人間とAIが同じRepositoryを別の方法で探索できることを試しています。

Humanには **今の興味から入れる入口** を。AIには **KnowledgeのStatus・Lifecycle・Relationを読み分けるためのStructure** を。

> **Human-friendly entrances. AI-friendly depth.**

## 3つのMap

- [Sitemap](./maps/sitemap.md) — **どこから入るか。**
- [Concept Map](./maps/concept-map.md) — **何と何が関係しているか。**
- [Knowledge State Map](./maps/knowledge-state-map.md) — **そのKnowledgeを、どの強さで読めばいいか。**

## If you remember only three things

ODDの用語を全部覚える必要はありません。最初は、この3つだけで十分です。

### Reality before Story

整った説明やTheoryより、実際に起きたことを優先します。RuleやInterpretationとRealityが衝突したら、Reality側から見直します。

→ [Reality First](./concepts/reality-first.md)

### Observation is not General Truth

一度起きたことは、その場で起きたObservationです。それだけでUser一般、Human一般、AI一般についてのTruthにはしません。

### Knowledge has State

書かれていることと、今も採用されていることは別です。Observation、Hypothesis、Candidate、Current、Legacyなど、そのKnowledgeが今どの状態にあるかを分けて扱います。

→ [Knowledge State Map](./maps/knowledge-state-map.md)

Co-Explorer、Meaning Authority、Human Fluctuationなどの名前は、必要になったときに読めば十分です。名前があること自体を、ODDの中心性や一般性の証拠として扱わないでください。

## Product Developmentではどう使っているか

```text
Observation
↓
Hypothesis / Candidate
↓
Experiment / Mock
↓
Reality Observation
↓
Design Decision
↓
Product Revision
↓
New Reality
```

Experimentは仮説を証明するためだけではなく、**新しいObservationを得るためのQuestion to Reality**でもあります。

→ [Observation to Design](./practices/observation-to-design.md)

## AIを「一人の万能AI」として扱わない

Ideasの開発では、AIを単なるTask Executorではなく、異なる認知位置を持つRoleとして使っています。

Product Owner、Assistant PM / Co-Explorer、Reviewer、Meta-Reviewer、Specialist、Meta-Specialist、Supportなどを分ける目的は、単なる分業ではありません。Context Pollution、Anchoring、Evaluation Bias、Optimization Pressureなどを扱うための **Cognitive Role Separation** です。

→ [AI Product Team](./practices/ai-product-team.md)

## ContextもDesign対象になる

すべてのAI Roleに同じContextを渡す必要はありません。Long-lived Contextが価値になるRoleもあれば、Fresh Contextが価値になるRoleもあります。

> **Continuity is role-dependent.**

→ [Handoff](./practices/handoff.md)

## Inheritance is continuity, not imitation.

Handoffでは、前のAIや過去のDocumentを再現することを目的にしません。

> **Current Repository / Current Observation > inherited interpretation**

過去のInterpretationはContextにはなります。Authorityにはなりません。

## Publicであることと、確定していることは別

> **公開する = 確定する**

ではありません。Public CandidateはPublicになってもCandidateのままです。

> **Visibility and epistemic status are separate dimensions.**

→ [Knowledge State Map](./maps/knowledge-state-map.md)

## Public ODDはIdeas Repositoryの公開版ではありません

IdeasとODDは別Repositoryとして管理します。

```text
Ideas → Internal Product Development / Reality Workbench
ODD   → Public Working Knowledge
```

Public ODDは、Internal Repositoryをコピーして秘密部分だけ削除したMirrorではありません。

> **Open the reasoning. Be selective with the recipe.**

Current Product UXの詳細、Behavior Calibration、Runtime Prompt、Implementation Specification、Instrumentation、Competitive Learningなどは公開対象外になる場合があります。User1以降のObservation / Experiment ResultもPublic ODDでは公開しません。

> **ODD can be open without making Ideas’ learning speed open.**

## User0について

Ideasでは、Product Owner自身がProductを使うとき、意識的に **User0** というRoleへ切り替えることがあります。目的は、設計者としての説明とUserとして実際に起きたReactionを少し分離して観察しやすくすることです。

User0本人についてはProduct Owner自身が公開判断できる範囲がありますが、第三者・組織・Product Competitive Detailには別のPublic Boundaryがあります。

> **User0 Observation ≠ User一般についてのObservation**

→ [User0 Selected Observations](./observations/user0/selected-observations.md)

## ODDという名前について

ODDは、初期には **Open Discovery & Development** と呼んでいました。

ここでいうDevelopmentには、問い・探索から新しい仕事・Product・行動・価値が生まれていくことと、AIと一緒にProductを作るAI-driven Developmentそのもの、両方のニュアンスがありました。

```text
Discovery
↓
Question / Possibility
↓
Human–AI Development
↓
New Work / Product / Value
↓
Reality
```

現在は **Open Discovery Design** という名前を使っています。名称の変化も含め、ODD自体がDevelopmentの中で変化してきたKnowledgeです。

→ [Ideas Origin](./cases/ideas-origin.md)

## 外のKnowledgeへ辿る

ODDには、既存の研究・Practiceと近いConceptがあります。ただし、SimilarityだけでODDのOriginやLineageを主張しません。

> **Related ≠ Equivalent ≠ Derived From**  
> **Similarity is not lineage.**

Public ODDでは網羅的なLiterature Reviewを抱え込むより、まずConceptへの入口を置きます。論文や書籍まで読みたい場合は、そのConceptから辿ってください。AIに比較や代表文献を尋ねても構いません。

→ [Related Concepts](./related-concepts/README.md)

## AIに読ませてください

このRepositoryは、AIに読ませることを想定しています。全部自分で読まなくても構いません。

> **Give this repository to an AI. Seriously.**

CandidateとPrincipleを区別した要約、弱い仮定の批判、自分のProjectへForkする際の再検証点などをAIに尋ねられます。

AI Reading Guideでは、単なるReading Orderだけでなく、Status・Uncertainty・Contradictionを保ち、SourceとInferenceを混同せず、ODD自体も誤り得るものとして読むためのInterpretation Protocolを試しています。

→ [AI Reading Guide](./ai-reading-guide/README.md)

## 分岐・改変歓迎です

ODDは、一つの正しいMethodologyとして中央管理することを目的としていません。一部だけ使う、前提を変える、別の名前を付ける、ODDとは違う結論へ進むことも歓迎します。

> **Forking can be part of Discovery.**

Contribution Backも必須ではありません。

→ [Forking Guide](./forking/README.md)

## License

Public ODD v0.1のKnowledgeは **Creative Commons Attribution 4.0 International（CC BY 4.0）** のもとで公開します。利用・共有・改変・Fork・商用利用が可能で、Attributionが必要です。変更した場合は、その旨も示してください。

→ [LICENSE](./LICENSE)

Software / executable codeを将来含める場合は、必要に応じて別のSoftware Licenseを指定します。

## ODDはまだ途中です

Cognitive Resource AllocatorやMutual PO / Product Firewallなど、まだ答えの出ていないQuestionもあります。完成するまで隠すのではなく、現在のStatusを付けて公開していきます。

## ODD itself meets Reality

Publicにした結果、分かりにくい、AIが誤読する、Forkしにくい、Classificationが重い、ConceptがRealityと合わないなら、ODD側を変えます。

> **Rules do not outrank Reality.**

Public ODDそのものもExperimentです。

```text
Working Knowledge
↓
Public
↓
Human / AI Use
↓
Critique / Fork / Misreading / Application
↓
External Reality
↓
New Observation
↓
Revision
```

完成したODDを公開しているのではなく、**ODDがRealityと接触しながら変わる場所を開いています。**
