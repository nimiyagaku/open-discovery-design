# ODD Generalization Notes

**Status: Exploring / Hypothesis**

This is not the foundation of ODD. It is a possible structure observed after the practices already existed.

## Why this note exists

ODDには、少なくとも複数のレベルのKnowledgeが混在しているように見えます。

- Ideasという特定Productの開発で生まれたPractice
- Human–AI systemで繰り返し現れるかもしれないPattern
- Human–AIに限定せず成立するかもしれないGeneral Model

これらを今すぐ分離・整理し切ることが目的ではありません。

むしろ、ODDのPracticeをそのまま一般理論へ持ち上げず、**どこまでがIdeas固有で、どこからがHuman–AI一般で、さらに何がより一般的な構造として残るのか**を観察するための構想です。

ODDは先に一般理論があり、そこからPracticeが導出されたものではありません。

先にRealityとFailureがあり、Practiceが生まれ、その後で薄い共通骨格のようなものが見え始めています。

## Working three-level view

### Level 3 — Practice

Ideas / ODDで実際に起きたFailure、Observation、Experiment、Design Decisionから生まれたWorking Knowledge。

Examples:

- Co-Explorer
- Fresh Review
- AI Product Team
- Knowledge State
- Observation to Design
- Handoff

ここが最もRealityに近いレベルです。

### Level 2 — Human–AI System

複数のPracticeを見たとき、Human–AI systemだからこそ繰り返し現れているように見えるPattern候補。

Candidate elements:

- Human × AI
- Reality
- Context
- Roles / Structure
- Meaning
- Knowledge

これはまだ確立したModelではありません。

Practice間で同じ構造が繰り返し見えるかを確認するための中間レベルです。

### Level 1 — General Model Candidate

Human–AIに限定しなくても成立するかもしれない、より薄い構造仮説。

Current candidate vocabulary:

- Agency
- Reality
- Context
- Structure
- Meaning
- Knowledge

ただし、これらを6つの独立した軸として扱うべきかは未解決です。

現在はむしろ、次のような非対称な関係の方が自然に見えています。

> Actors interact with Reality under constraints, producing Meaning and Knowledge that alter subsequent interaction.

別の言い方をすると、

- AgencyがRealityと相互作用する
- ContextとStructureがその相互作用を制約する
- MeaningとKnowledgeがその相互作用から生成・更新される
- 生成されたMeaning / Knowledgeが、次のContextや相互作用へ戻る

という循環です。

## Practice → Pattern → Model

現在の仮説では、一般化は次のように進みます。

```text
Practice
  ↓ repeated structure?
Pattern
  ↓ survives beyond Human–AI?
Model
```

ただし、これはKnowledgeの「昇格」ではありません。

上位に行くほど確からしくなるわけではなく、むしろRealityから離れるため、抽象化に伴う不確実性は増えます。

- Practiceは最も具体的で、Realityに近い
- Patternは複数Practiceからの抽象化
- Modelはさらに弱いHypothesis

一般化できないPracticeが劣っているわけでもありません。

Ideas固有だからこそ価値があるKnowledgeもあります。

## Model → Pattern → Practice

逆方向もありえます。

General Model Candidateが正しいと仮定したとき、新しいExperimentやFailure候補を導ける可能性があります。

たとえば、

> StructureがAgencyの判断へ影響するなら、generationとevaluationを同じContextに置いたとき何が起きるか？

> Knowledgeが次のContextへ再投入されるなら、古いKnowledgeのStateを失ったとき何が起きるか？

といった問いです。

この場合も、ModelはRealityより上位のRuleではありません。

Modelの役割は答えを決めることではなく、**Realityへ新しいQuestionを投げること**です。

Modelから予測されたFailureがRealityで観察されなければ、Model側を疑います。

## Keep the scars

一般化するとき、Conceptが生まれた傷跡を消さないことが重要です。

Generalizationによって残したい情報:

- Originating Reality
- どのProduct Realityで問題が強く表面化したか
- 最初は何を正しいと思っていたか
- 何がうまくいかなかったか
- 何によって修正されたか
- 一般化するときに何を捨てたか
- まだProduct固有かもしれない部分

きれいな上位概念だけを残すと、Conceptが最初から普遍的原理として存在していたように見えます。

ODDでは、一般化しても元のFailureやProduct-specific pressureへの帰り道を残します。

## Product-specific pressureを消さない

あるConceptがHuman–AI一般へ持ち出せそうに見えることと、**なぜODDでそのConceptが強く必要になったか**は別です。

Human–AI一般に成立しうる構造が、特定Productの性質によって強く増幅され、Conceptとして表面化した可能性があります。

したがってGeneralizationでは、少なくとも次の二つを分けて残します。

> Where might this generalize?

> Why did it become salient here?

### Example — Meaning Authority

Meaning Authorityは、Human–AI一般にも関係する可能性があります。

AIを含む他者から影響を受けても、HumanがMeaningを訂正・更新・再解釈・置換できることは、Ideas以外でも重要になりえます。

一方で、Ideasは探索を通じてHuman自身の意味や自己理解が変化することをProduct Experienceの中心近くに置いています。

そのため、AIが意味形成へどこまで介入するかという問題が、Ideasでは特に強く表面化しました。

つまり、

> Human–AI一般に成立しうる構造
> ≠
> その構造がODDで重要になった理由

です。

Meaning Authorityを一般化できる可能性があっても、現在のConceptの形や感度にはIdeas固有のProduct Realityが含まれています。

また、Meaning Authority自体も最初から現在の形だったわけではありません。

初期にはMeaningを守ることがAI Influenceを弱める方向へ寄りやすく、その後、強いInterpretationが良いExperienceを生むRealityによって、Influenceを避けることよりMeaningを訂正可能に保つことへ重心が移りました。

このRevisionを消して、現在のDefinitionだけを一般化しないことが重要です。

## Other concepts to test

この3層で、今後いくつかのConcept / Practiceを試しに見直せます。

### Fresh Review / AI Product Team

Questions:

- Ideas固有のPracticeか？
- Human–AI Product Development一般で繰り返すPatternか？
- より一般にはContext / StructureによるAgency配置の問題として扱えるか？

注意:

Fresh ContextはMissing Contextではありません。

制作過程のContextを切ることと、評価に必要な最新情報を渡さないことは別です。

### Human Fluctuation

Questions:

- Ideasの探索Productだから特に強く問題化されたのか？
- Human–AI personalization一般でも成立するか？
- より一般には、Past StateをCurrent Agencyへ固定しない問題として扱えるか？

### Knowledge State

Questions:

- AIによるKnowledge再利用が強くなるほど一般性が高まるか？
- Current / Legacy、Hypothesis / Decisionなどの区別はHuman–AI以外でも必要か？
- ContextとKnowledgeは本当に別要素か？

### Reality First

Questions:

- IdeasのProduct Development RuleとしてのReality Firstと、一般的なRealityとの関係は同じか？
- Realityは単なるTheoryの検証先ではなく、Valueが生成される場所でもあるという特徴を一般化できるか？

### Co-Explorer

Questions:

- Human–AI exploration固有のRole Designか？
- より一般にはAgency間のMeaning formationへの介入設計として扱えるか？
- Product-specificな「探索して自分について何か見つける」という価値をどこまで切り離せるか？

## Open questions

この構想はまだかなり不安定です。

特に次を疑います。

### AgencyとStructureは独立か？

Roleや権限、配置はAgencyそのものを構成している可能性があります。

StructureをAgencyの外側の制約として扱うのが正しいとは限りません。

### ContextとKnowledgeの境界は何か？

Knowledgeは保存されたもの、Contextは現在Activationされているもの、と区別できるかもしれません。

しかしKnowledgeがContext化する過程まで含めると、二つを独立要素として置く必要がない可能性もあります。

### Meaningは独立要素か？

MeaningはAgencyとRealityの相互作用から生成されるものかもしれません。

独立したBoxとして置くより、関係や生成物として扱う方が自然な可能性があります。

### KnowledgeはMeaningの保存形なのか？

KnowledgeにはObservation、Decision、EvidenceなどMeaning以外も含まれます。

MeaningとKnowledgeの関係はまだ粗いです。

### Human–AI以外でも成立するか？

Team、Organization、Human–Human、tool-mediated workなどに持ち出したとき、同じ構造が本当に残るかは未確認です。

### AIによる後付けの統合ではないか？

複数のPracticeを見たAIが、後から綺麗な共通Theoryを作っているだけの可能性があります。

「すべて説明できる」ことを、このModelのEvidenceにしません。

本当に価値があるかを見るには、このModelからまだ観察していないFailureやExperimentを導き、Realityで壊せるかを見る必要があります。

## Do not assume

- ODDがこのGeneral Modelから設計されたわけではありません。
- このModelはODDのFoundationではありません。
- すべてのODD Practiceに共通祖先があるとは限りません。
- Practiceを一つのTheoryへ無理に統合しません。
- Level 1ほど真・成熟・重要という意味ではありません。
- Ideas固有のKnowledgeが一般Knowledgeより劣るわけではありません。
- GeneralizationでProduct-specific pressureを消しません。
- Current Definitionだけを残し、FailureやRevisionの傷跡を消しません。
- このModelを新しいObservationへ自動適用しません。
- ODDで説明できることと、ODDで説明すべきことは別です。

## Current stance

現時点では、ODDの下に確立したGeneral Theoryがあるとは考えていません。

より正確には、

> **バラバラに生まれたPracticeの下に、薄い共通骨格があるように見え始めている。**

というObservation / Hypothesisです。

この骨格が本当に存在するのか、どこまで一般化できるのか、どのPracticeはそもそも同じ構造ではないのかを、今後のRealityで確認します。

一般化すること自体を目的にはしません。

General Modelが役に立たなければ、捨てます。
