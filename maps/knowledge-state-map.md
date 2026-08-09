# Knowledge State Map

**Epistemic Status:** Navigation / Knowledge Architecture Candidate  
**Lifecycle:** Current / Exploring  
**Summary:** Public ODD内のKnowledgeを「何として知っているか」「今どう扱われているか」「どこまで公開されているか」を分けて読むためのMap。

## Why This Map Exists

Public ODDには、Observation、Hypothesis、Candidate、Practice、Principle、Open Question、Legacyなど、異なる種類・強さ・状態のKnowledgeが同時に存在します。

> **「ODDに書いてあること」を全部同じ強さで読まない。**

## Four Different Questions

```text
Navigation       → どこに置かれているか
Epistemic Status → 何として知っているか
Lifecycle        → 今どう扱われているか
Visibility       → どこまで公開されているか
```

> **Navigation Category ≠ Epistemic Status**

`concepts/` にあるからPrinciple、`practices/` にあるから証明済みMethod、という意味ではありません。

## Epistemic Status

### Observation
実際に観察されたこと。

> Observation ≠ Explanation ≠ General Truth

### Hypothesis
Observationを説明するための仮説。

### Candidate
現在、有用そうなので探索・利用している考え方。

> Currently useful ≠ universally established.

### Practice
現在、実際のProduct Developmentや運用で使っている方法。

> Used ≠ Proven.

### Principle
複数のObservationやRealityとの接触を経て、比較的安定して参照している考え方。ただしImmutable Lawではありません。

### Open Question
現在まだ答えが出ていないQuestion。Documentation不足とは限りません。

## This Is Not a Maturity Ladder

Observation → Hypothesis → Candidate → Practice → Principle のような自動昇格モデルではありません。

RealityはKnowledgeを Strengthen / Modify / Narrow / Suspend / Reopen / Reject できます。

## Lifecycle

- **Current** — 現在参照・利用している
- **Exploring** — 現在特に積極的に試している
- **Dormant** — 否定されていないが積極的に追っていない
- **Superseded** — より新しいKnowledgeやDesignに置き換えられた
- **Legacy** — 過去のStageを理解するために残している

> **Legacy ≠ Wrong.**  
> **Legacy ≠ Current Source of Truth.**

## Visibility

- **Internal** — Ideas内部などにのみ存在
- **Public** — Public ODDで比較的直接公開
- **Public Abstracted** — Internal KnowledgeからPublic Representationを生成

> **Public Abstracted ≠ Redacted Mirror**

## Visibility Does Not Change Epistemic Status

```text
Internal Candidate
↓ Publish
Public Candidate
```

であって、Public Principleへ自動昇格するわけではありません。

> **公開することは、確定することではありません。**

公開とは、外部からも観察・批判・再利用・Fork可能にすることです。

## Representation / Provenance

必要なDocumentでは selected / anonymized / abstracted / synthesized などを明示できます。ただしv0.1では必須Metadataにしません。運用負荷を増やさないためです。

## Publication Basis Can Matter

User0はProduct Owner本人なので、本人に関するObservationには本人が公開判断できる範囲があります。一方で、第三者・組織・Product Competitive Detailなどは別のPublic Boundaryを持ちます。

## Minimal Metadata

基本候補は次の程度です。

```yaml
epistemic_status: Candidate
lifecycle: Current
summary: "..."
```

必要な場合のみ `representation: synthesized` などを追加します。

> **Knowledge Architectureの完全性より、継続できる運用を優先する。**

## Common Misreadings

- Observation → General Truth にしない
- Candidate → Rule にしない
- Practice → Universal Method にしない
- Public → Confirmed にしない
- Legacy → Wrong にしない
- Public Abstracted → Primary Source にしない
- Principle → Reality Override にしない

AIにもこのDifferenceを保持することを期待します。

→ [AI Reading Guide](../ai-reading-guide/README.md)

## The Map Itself Has a State

このArchitecture自体もCandidateです。Human / AI UseによってStatus、Lifecycle、Metadataが役立たないと分かれば変更します。

> **Rules do not outrank Reality.**
