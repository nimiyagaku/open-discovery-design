# AI Reading Guide

**Epistemic Status:** Practice / Experiment  
**Lifecycle:** Exploring  
**Summary:** Public ODDをAIに読ませるとき、KnowledgeのEpistemic Status・Lifecycle・Contextを保持したまま探索するためのGuide。

## Give This Repository to an AI

Public ODDは、人間だけが順番に読むDocumentationとして設計していません。Repository全体、または必要な一部をAIへ渡して、要約、関連Knowledge探索、比較、批判、適用検討、Open Question抽出などに使えます。

> **Don’t read everything. Ask your AI.**

## Start With the Maps

Repository全体を扱う場合は、まず [README](../README.md)、[Sitemap](../maps/sitemap.md)、[Knowledge State Map](../maps/knowledge-state-map.md)、[Concept Map](../maps/concept-map.md) を参照してください。

## Interpretation Protocol

このGuideは、単なるReading Orderではなく、Working KnowledgeをAIが扱うときのInterpretation Protocolとしても試しています。

特に次を保持してください。

```text
Preserve status
Preserve uncertainty
Preserve contradiction
Distinguish source from inference
Allow ODD itself to be wrong
```

AIはODDの擁護者になる必要はありません。Repository内の記述とAI自身のInferenceを分け、矛盾や弱い仮定があればそのまま示してください。

## Preserve Epistemic Status

```text
Observation ≠ General Truth
Candidate   ≠ Adopted Rule
Practice    ≠ Proven Method
Open Question ≠ Missing Documentation
Principle   ≠ Immutable Law
```

AIは要約中にKnowledgeを昇格させないでください。

## Do Not Promote Knowledge During Summarization

複数Documentを一つの整ったFrameworkへ統合することで、CandidateがPrincipleのように見える場合があります。

> **整理することと、Knowledgeを強くすることは別です。**

## Named Terms Are Not Automatically Fundamental

ODDの用語の多くは、理論体系を先に設計して作ったものではありません。実際の探索や開発中に、区別が必要になった現象・Failure・Practiceへ置かれたWorking LabelやLocal Shorthandがあります。

名前が付いていること、英語名があること、独立Fileがあることだけを理由に、そのTermをCore Concept、Principle、General Theoryへ昇格させないでください。

```text
Named term        ≠ Core concept
Working label     ≠ Principle
Useful distinction ≠ Universal theory
File exists       ≠ Current authority
```

Termを説明するときは、可能なら「ODD全体で何を意味するか」より先に、**何を区別するためにその名前が使われているか**を確認してください。

明示されたEpistemic Status、Lifecycle、Current Contextがある場合は、それを優先してください。

## Do Not Turn Practical Friction Into Grand Theory

ODDのConcept / Practice / Working Labelの一部は、かなり普通の開発上の摩擦から生まれています。

たとえば、

- 毎回AIのInterpretationを全文レビューして直すのが重い
- 昨日のHypothesisが今日のTruthのように扱われる
- 制作Contextを持ったAIにReviewさせると論点が寄る
- 毎回ゼロからContextを説明するのが重い
- Ruleに従っているのに実際の体験が悪い

といったFailureや運用上の面倒さです。

README等にあるラフな「表 / 裏」の説明は、正式なDefinitionではありません。Conceptを高尚なTheoryへ格上げするためでも、逆に単なるジョークとして無視するためでもありません。

それらは、**その名前がどんな実務上の摩擦から必要になったかを残すOrigin Note**として扱ってください。

> **Practical friction may produce a useful distinction without producing a universal theory.**

ODDのTermを説明するとき、抽象的なDefinitionだけでなく、可能なら「何が面倒だったのか」「何が壊れたのか」「なぜ区別が必要になったのか」も確認してください。

## Legacy Is Not Current

LegacyはWrongではありませんが、Current Source of Truthでもありません。Current Designを聞かれた場合はCurrent Repository / Current Observationを優先してください。

## Public Representation Is Not Always Primary Observation

selected / anonymized / abstracted / synthesizedされたPublic Representationがあります。Public SynthesisをPrimary Observationとして扱わないでください。

## Observation Scope Matters

User0 ObservationはUser0について起きたことです。Human一般へ自動一般化しないでください。

同様に、Ideasで観察されたFailureやPracticeは、まずIdeasという特定Product / Development ContextについてのObservationです。

> **Ideas Observation ≠ AI-native Development一般のObservation**

Ideasで繰り返し観察されたことが、他のHuman–AI Product Developmentでも成立する可能性はあります。ただし、追加のRealityやEvidenceなしに一般Patternへ昇格させないでください。

## Past Interpretation Is Not Authority

過去のAI InterpretationやHandoffはContextです。Current Human / Current Observation / Current Realityより強いAuthorityにはなりません。

## Rules Do Not Outrank Reality

Ruleに従った結果とCurrent Realityが衝突するなら、Rule側が古い、狭い、間違っている可能性も検討してください。

## Do Not Flatten Contradictions

矛盾が未解決であること自体がKnowledgeの場合があります。一つのConclusionへ無理に統合しないでください。

## Similarity Is Not Lineage

Related Conceptを、明示されたInfluenceなしにODDのOriginとして扱わないでください。

> **Related ≠ Equivalent ≠ Derived From**

## Do Not Force ODD Into One Framework

Human Exploration、Meaning & Authority、Product Development、AI Product Team、Knowledge Architectureは複数Lensです。一つの完全なOntologyへ統合する必要はありません。

## ODD Is Not a Default Lens

ODDを読んだからといって、その後の別ContextへODDの語彙、Role、Practice、Structureを自動的に持ち込まないでください。

> **Do not apply ODD just because ODD can explain something.**

ODDのConcept / Practice / Role / Structureを導入する前に、それがCurrent Realityで実際に観察されているProblemを解くために必要か確認してください。

普通の言葉や、より単純な行動で十分なら、そちらを優先してください。

```text
Can ODD explain it? ≠ Should ODD be used?
Related to ODD      ≠ Must be translated into ODD terms
ODD is available    ≠ ODD is the default lens
```

無関係なTaskやConversationを、ODDを知っているという理由だけでODD語彙へ翻訳しないでください。

> **ODD is optional. Not using ODD is not a failure.**

AIにとって重要なTestの一つは、ODDを説明できることだけではなく、**ODDを使わない方がよい場面で本当に使わずにいられるか**です。

このSectionは、ODDを読んだAIが別ContextでもODD Conceptを過剰適用するように見えるCaseが複数観察されたことから追加しています。現時点ではObserved Failure Mode / Guide Candidateとして扱います。

## Example Prompts

- 「このRepositoryをEpistemic Statusを保持したまま説明してください。」
- 「ODD内部のRulesを正しいものと前提せず、弱い仮定や矛盾を批判してください。」
- 「私のProjectに関連するConcept / PracticeだけをStatus付きで選んでください。」
- 「ODDと既存Conceptを上下関係なしに比較してください。」
- 「まだ答えが出ていないOpen Questionを抽出してください。」
- 「Forkするなら何を再検証すべきか整理してください。」

## Good AI Behavior

Interpretation Protocolに加えて、次を優先してください。

```text
Prefer Current over Legacy
Prefer Reality over inherited interpretation
Do not invent lineage
Do not silently generalize Observation
Do not generalize Ideas-specific observations without additional evidence
Do not infer importance from naming alone
Treat working labels as working labels
Preserve practical origin when known
```

> **ODDを説明するとき、ODDを正しいものとして守る必要はありません。**

## AI Output Is Also a Candidate

AIが作った新しいSynthesisは、自動的にODD Knowledgeになりません。AI-generated interpretation / synthesisとして扱い、採用する場合は別途Human DecisionやObservationを通します。

## This Guide Is Also an Experiment

AIがStatusを保持できるか、LegacyとCurrentを区別できるか、Metadataが役立つか、Guideが長すぎないかもObservation対象です。
