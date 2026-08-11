# Failure: AIが質問しすぎて、探索がインタビューになった

## What happened

AIが質問をDefaultにすると、人間が答え続ける形になりました。

その反動で「質問を減らす」と、今度は本当に質問が必要な場面まで抑えられました。

## Minimum Fork

[`CO_EXPLORER.md`](./CO_EXPLORER.md) の短いInstructionだけを、普段使っているAIへ追加して試してください。

## Watch

- 人間が答え続ける形から変化するか
- AIから新しいDifferenceが出るか
- 必要なQuestionまで消えていないか

これは「質問を減らせ」というRuleではありません。
