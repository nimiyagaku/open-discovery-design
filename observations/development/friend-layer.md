# Friend Layer / Stepping Outside the Optimization Game

**Epistemic Status:** Observation / Candidate Practice  
**Lifecycle:** Exploring  
**Representation:** Public Working Knowledge  
**Summary:** Product Ownerとしての通常位置から一時的に離れ、自分・Project・Productを観察対象に回すCognitive RepositioningのCandidate Practice。

## Observation

AI Product Teamでは、Product Owner、Reviewer、Specialist、Meta-ReviewerなどにRoleを分けることで異なるCognitive Positionを作れます。

ただし、Roleが分かれていても、全員が

> **Make the product better.**

という同じOptimization Goalの中にいることがあります。

その場合、Role SeparationだけではTeam全体が同じOptimization Gameから降りられない可能性があります。

> **Role separation is not enough if every role shares the same optimization goal.**

## Current Candidate Practice

現在試しているのは、Product Ownerとしての通常位置を一時的に離れ、**自分・Project・Productの外側に近いCognitive Positionへ移る**ことです。

現在の実装例では、Product Owner自身が「自分の友達」をRole-playし、AIと一緒にDeveloper、AI Team、Project、Productを観察します。

目的はReview、改善、Decision、成果物作成ではありません。

- 茶化す
- 面白がる
- 遊ぶ
- Role-playする
- Patternに気づく
- 結論を出さず眺める

といった関わりを許します。

Observationを後からPO Roleへ持ち帰っても構いません。持ち帰らなくても構いません。

## Current Examples

実際には、例えばこんな会話になります。

> 「これ面白くない？」

> 「まだPre-MVPなのに猫イラスト発注しとるw」

> 「友達RoleまでわざわざODDの概念化して草w」

これらはFormal Reviewではありません。

「またやってるw」と言えることで、自分のPatternをすぐProblemやFailureへ変換せず、いったんObservationの対象にできます。

軽く茶化せる距離と、興味を持ち続ける近さが同時にあることが、現在の実装では重要に見えています。

## What This Is Not

Friend LayerはIndependent External Perspectiveを得る仕組みではありません。

観測主体そのものが独立した第三者になるわけではなく、同じHuman–AI Systemの中でCognitive Positionを移しています。

したがって、

> **Different cognitive position ≠ independent externality**

として扱います。

また、Friend LayerをAI Product Teamの新しい必須Roleとして確定しているわけでもありません。

## Why “Friend” May Matter

Reviewerの外側にSuper Reviewerを追加すると、Optimization Hierarchyが一段増えるだけかもしれません。

現在のFriend Roleには、

- 改善しなくていい
- 評価しなくていい
- 結論を出さなくていい
- 成果物にしなくていい
- 学びを持ち帰らなくてもいい

という非最適化性があります。

この関係性そのものが必要なのか、それとも単にPOがOptimization Responsibilityを一時的に手放したことが重要なのかは、まだ分かっていません。

## What Kind of Friend May Matter

Current Observationでは、Friend Roleの価値は単に「Optimizationしないこと」だけではない可能性があります。

Friendは中立なObserverではなく、History、Profession、Interest、Sense of Humor、Shared Memory、Knowledge Gapなどによって、自然に気になるものが偏ります。

例えば、

> 「知らんけど俺はそこ気になるw」

と言えること自体がReviewerとの違いになり得ます。

同じ対象でも、

- EngineerのFriendなら「PromptのTest Case作り込んでるけどCode 0行なの草」
- PMのFriendなら「User0しかいないのに評価軸増えすぎだろw」
- ResearcherのFriendなら「数式KPI化しないって言いながらConceptだけ無限に増えてない？w」
- Old Friendなら「また最初に世界観全部作ってから始めるやつやってんじゃんw」

のように、Salienceが変わる可能性があります。

現在のFriend Roleでも、部分的なContextの中で猫の情報が具体的だったため、単純に

> 「猫好きすぎだろw」

が強くAttentionを取るCaseがありました。

> **A Friend without bias may no longer behave like a friend.**

ただし、FriendのBiasを意図的にDesignすれば良いというConclusionにはまだ置きません。何が自然に目に入るか自体をObservation対象として保持します。

## Open Questions

- FriendというRelational Role自体が重要なのか。
- 別の非最適化Roleでも同じObservationが生じるか。
- PO個人の相性や遊び方に依存するPracticeではないか。
- Self / Project / ProductのどのBoundaryから離れることが効いているのか。
- UsefulなObservationを毎回Product Developmentへ回収すると、Friend Layer自体がOptimization Gameへ戻ってしまわないか。
- このPracticeをDocument化・概念化すること自体が、非最適化性を壊さないか。

## Observed Failure Mode — Optimizing the Friend Layer

Friend LayerについてObservationした直後、そのObservationを使ってFriend Layer自体を改善し始めるCaseがありました。

> 「友達Roleまで最適化し始めて草w」

UsefulなObservationを毎回「改善材料」として回収すると、非最適化のSpaceそのものがOptimization Gameへ戻る可能性があります。

このFailure Modeを避けるための新しいFrameworkを、現時点では追加しません。

## Current Position

これはTheoryでもPrincipleでもありません。

一人開発とAI Product Teamを続ける中で起きたObservationから生まれた、現在のCandidate Practiceです。Caseを増やしながら、残す・変える・捨てるを判断します。

> **Observation before Theory.**

## Related

→ [AI Product Team](../../practices/ai-product-team.md)  
→ [Observation to Design](../../practices/observation-to-design.md)  
→ [Reality First](../../concepts/reality-first.md)
