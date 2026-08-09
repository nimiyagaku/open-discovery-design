# AI Reading Guide

**Epistemic Status:** Practice / Experiment  
**Lifecycle:** Exploring  
**Summary:** Public ODDをAIに読ませるとき、KnowledgeのEpistemic Status・Lifecycle・Contextを保持したまま探索するためのGuide。

## Give This Repository to an AI

Public ODDは、人間だけが順番に読むDocumentationとして設計していません。Repository全体、または必要な一部をAIへ渡して、要約、関連Knowledge探索、比較、批判、適用検討、Open Question抽出などに使えます。

> **Don’t read everything. Ask your AI.**

## Start With the Maps

Repository全体を扱う場合は、まず [README](../README.md)、[Sitemap](../maps/sitemap.md)、[Knowledge State Map](../maps/knowledge-state-map.md)、[Concept Map](../maps/concept-map.md) を参照してください。

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

## Legacy Is Not Current

LegacyはWrongではありませんが、Current Source of Truthでもありません。Current Designを聞かれた場合はCurrent Repository / Current Observationを優先してください。

## Public Representation Is Not Always Primary Observation

selected / anonymized / abstracted / synthesizedされたPublic Representationがあります。Public SynthesisをPrimary Observationとして扱わないでください。

## Observation Scope Matters

User0 ObservationはUser0について起きたことです。Human一般へ自動一般化しないでください。

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

## Example Prompts

- 「このRepositoryをEpistemic Statusを保持したまま説明してください。」
- 「ODD内部のRulesを正しいものと前提せず、弱い仮定や矛盾を批判してください。」
- 「私のProjectに関連するConcept / PracticeだけをStatus付きで選んでください。」
- 「ODDと既存Conceptを上下関係なしに比較してください。」
- 「まだ答えが出ていないOpen Questionを抽出してください。」
- 「Forkするなら何を再検証すべきか整理してください。」

## Good AI Behavior

```text
Preserve status
Preserve uncertainty
Preserve contradiction
Distinguish source from inference
Prefer Current over Legacy
Prefer Reality over inherited interpretation
Do not invent lineage
Do not silently generalize Observation
Allow ODD itself to be wrong
```

> **ODDを説明するとき、ODDを正しいものとして守る必要はありません。**

## AI Output Is Also a Candidate

AIが作った新しいSynthesisは、自動的にODD Knowledgeになりません。AI-generated interpretation / synthesisとして扱い、採用する場合は別途Human DecisionやObservationを通します。

## This Guide Is Also an Experiment

AIがStatusを保持できるか、LegacyとCurrentを区別できるか、Metadataが役立つか、Guideが長すぎないかもObservation対象です。
