# Failure: 過去の判断をAIが現在にも適用し続けた

## What happened

過去に妥当だったKnowledgeが残っていると、AIが現在の判断でも同じ重さで参照することがありました。

## Minimum Fork

まず2つだけに分けます。

- [`CURRENT.md`](./CURRENT.md) — 今の判断に使ってよいもの
- [`PAST.md`](./PAST.md) — 残しておくが、現在の判断には自動で使わないもの

複雑なTaxonomyは不要です。

## Watch

- 古い判断が現在のRuleとして復活しにくくなるか
- 過去を必要なときには参照できるか
- Currentへ置くものが増えすぎていないか
