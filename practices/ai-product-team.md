# AI Product Team

**Epistemic Status:** Practice / Candidate  
**Lifecycle:** Current / Exploring  
**Representation:** Public Synthesis  
**Summary:** AIを単なるTask分担ではなく、異なる認知位置とContext Boundaryを持つRoleとして使うPractice。

## Core Idea

> **AI Product Team is not an org chart for distributing tasks; it is Role Design for seeing Product / Reality from different cognitive positions.**

目的は単なる分業ではありません。

- Cognitive Loadを分散する
- Independent Perspectiveを作る
- Context Pollutionを減らす
- Anchoringを減らす
- Consistency Pressureを減らす
- Domainを分離する
- Optimization PressureへのCounterweightを置く

## Current Roles

### Product Owner
Product Purpose、Decision、Reality上のResponsibilityを引き受けます。

Operational Rulesには広いOverride Authorityがあります。内部では比喩的に「PO can sudo operational rules」と捉えることがあります。

```text
Operational Rules → PO may override
Protective Guardrails → PO cannot necessarily override
```

Authorityはunrestricted self-exemptionではありません。Protective GuardrailsはUser、Product、PO本人を重大なHarmから守るため、POのOperational Authorityの外に置かれる場合があります。

また、POは実際にはOverrideをほとんど使っていません。Override自体にもDecision、Re-alignment、Communication Costがあるためです。

> **PO can override ≠ PO routinely overrides.**

### Assistant PM / Co-Explorer
Long-lived Contextを持ち、Project Continuityと探索を支えます。

> **Inheritance is continuity, not imitation.**

### Reviewer
Output / Decisionを別位置から評価します。

### Meta-Reviewer
Evaluation Systemそのものを評価します。

> **Rulesを守ろうとした結果、Productを壊していないか。**

### Specialist
一つのDomainを深く見ます。

### Meta-Specialist
複数Domain間のRelation、Trade-off、Boundaryを見ます。

### Support
Optimization PressureへのCounterweightです。「今日はここまで」「未解決のまま置く」「休む」「楽しむ」といった選択肢を戻します。

Product Ownerは普段、このRoleを **「甘やかし担当」** と呼んでいます。

Supportは単なるPraise Roleではなく、Product Owner自身のReactionやAffective Calibrationを探索するSpaceにもなり得ます。

## Context Is Role-Dependent

Assistant PM / Co-ExplorerはContinuityのためLong-lived Contextを持つ一方、Reviewer、Meta-Reviewer、Specialist、Meta-SpecialistにはFresh / Selective Contextを意図的に与える場合があります。

Fresh ContextはLossではなくFeatureになり得ます。

> **Continuity is role-dependent.**

### Context Boundary

各Roleについて、

- What should this role know?
- What may it know?
- What may be useful not to know yet?

を考えます。

同じAIが長いContextの中でGenerateとReviewを繰り返すと、以前のFramingを自己強化する可能性があります。Role SeparationはDisagreementやTensionを許容します。

## Future / Open Candidate — Cognitive Resource Allocator

AIがResearch、Generation、Implementation、Reviewを高速化すると、Human側のDecision CostがBottleneckになり得ます。

```text
AI execution speed ↑
→ candidates / outputs / feedback ↑
→ Human decision demand ↑
→ review / prioritization / role switching ↑
→ Human cognitive bottleneck
```

Questionは「Humanが遅いからAIに決めさせる」ことではありません。

> **How can Human retain Decision / Meaning Authority while managing the cognitive cost Humans must pay?**

また、Human自身もPO、Designer、Developer、Reviewerなど複数Roleを切り替えます。対象はTask Allocationだけではなく、

> **Role Allocation + Context Allocation**

です。

HumanをApproval Machineにしない一方、Human AuthorityをAIへ静かに移しすぎないBoundaryを探索しています。

現在、独立RoleなのかAssistant PM / Meta-ReviewerなどのCapabilityなのかは未解決です。

## Future / Open Candidate — Mutual PO / Product Firewall

> **POからProductを守り、ProductからPOも守る。**

PO PreferenceがProductをPOへOverfitさせる可能性があります。一方、KPI、Feedback、Review、Optimization PressureがPOのCognitionや生活へ入りすぎる可能性もあります。

これは単なる情報遮断ではなく、**どのInfluenceを、いつ通すか**というBoundaryのQuestionです。

Role、Process、Guardrail、Firewallのどれとして実装するかは未解決です。

## Related Concepts

Multi-agent Systems、Separation of Concerns、Independent Review、Context Engineering、Distributed Cognitionなどは理解の足場になり得ます。

> **Related ≠ Equivalent ≠ Derived From**
