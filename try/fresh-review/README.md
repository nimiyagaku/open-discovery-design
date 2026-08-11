# Failure: 作ったAIにそのままレビューさせたら、レビューが作者寄りになった

## What happened

制作中の理由や迷いを知っているAIに、そのまま成果物のReviewを頼むと、そのContextに引っ張られることがありました。

## Minimum Fork

1. 制作Sessionとは別の新しいSessionを作る。
2. [`REVIEWER.md`](./REVIEWER.md) を渡す。
3. 成果物・Review目的・必要な評価条件だけを渡す。

## Watch

- 指摘の種類や強さが変わるか
- 制作者の意図を擁護する説明が減るか
- 逆に、必要なContext不足で誤読が増えないか

Fresh Contextは独立した外部視点を保証しません。
