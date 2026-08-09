# Open Discovery Design

**AIと作っていたら、考え方や開発の仕組みまで育ってきた。**

Open Discovery Design（ODD）は、最初から完成したFrameworkとして設計されたものではありません。

IdeasというProductを、人とAIで実際に作りながら、

- 人とAIはどう一緒に考えられるか
- AIが意味形成へ関わるとき、何を守るべきか
- ObservationをどうProductへ戻すか
- AIをTeamとして使うとき、RoleやContextをどう分けるか
- 開発中に生まれたKnowledgeをどう残し、引き継ぎ、公開するか

といったQuestionに向き合う中で、少しずつ析出してきたWorking Knowledgeです。

> **思想を先に完成させてProductへ適用したというより、Productを作っていたら、思想・設計・チーム・運用が少しずつ析出してきた。**

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

## まず全部読む必要はありません

ODDを理解するために、最初から全部読む必要はありません。今の興味から入ってください。

- 「ODDって何？」 → [Sitemap](./maps/sitemap.md)
- 人とAIがどう一緒に考えるか → [Co-Explorer](./concepts/co-explorer.md)
- AIが意味へ影響することが気になる → [Meaning Authority](./concepts/meaning-authority.md)
- AIでProduct Developmentする方法に興味がある → [AI Product Team](./practices/ai-product-team.md)
- 理論より、実際に起きたことを見たい → [User0 Selected Observations](./observations/user0/selected-observations.md)
- Knowledgeがどう更新されるか → [Observation to Design](./practices/observation-to-design.md)
- AIにこのRepositoryを読ませたい → [AI Reading Guide](./ai-reading-guide/README.md)
- ODDを自分のProjectへ持っていきたい → [Forking Guide](./forking/README.md)

## Human-friendly entrances. AI-friendly depth.

Public ODDでは、人間とAIが同じRepositoryを別の方法で探索できることを試しています。

Humanには **今の興味から入れる入口** を。AIには **KnowledgeのStatus・Lifecycle・Relationを読み分けるためのStructure** を。

> **Human-friendly entrances. AI-friendly depth.**

## 3つのMap

- [Sitemap](./maps/sitemap.md) — **どこから入るか。**
- [Concept Map](./maps/concept-map.md) — **何と何が関係しているか。**
- [Knowledge State Map](./maps/knowledge-state-map.md) — **そのKnowledgeを、どの強さで読めばいいか。**

## Core Concepts

### Co-Explorer
AIは意味を完成させる存在でも、ただ受け身でいる存在でもない。Contextに応じて探索へ参加し、必要なら何もしない。

→ [Co-Explorer](./concepts/co-explorer.md)

### Meaning Authority
AIからInfluenceを受けないことではなく、**Meaningを後から修正できる状態を保つこと。**

→ [Meaning Authority](./concepts/meaning-authority.md)

### Reality First
良いDialogueや整ったTheoryが、Realityより強いとは限りません。

> **Observation before Theory.**  
> **Reality before Story.**

→ [Reality First](./concepts/reality-first.md)

### Human Fluctuation
HumanのInterest、Meaning、Readiness、Attentionは動きます。変化したこと自体を、自動的にFailureとは扱いません。

→ [Human Fluctuation](./concepts/human-fluctuation.md)

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

## AIに読ませてください

このRepositoryは、AIに読ませることを想定しています。全部自分で読まなくても構いません。

> **Give this repository to an AI. Seriously.**

CandidateとPrincipleを区別した要約、弱い仮定の批判、自分のProjectへForkする際の再検証点などをAIに尋ねられます。

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
