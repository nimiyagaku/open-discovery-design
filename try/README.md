# Try one ODD failure

ODDを全部理解してから使う必要はありません。

下の中に「これ、自分のAI利用でも起きている」と思うものがあれば、そのケースだけ持っていって試してください。

ここにあるのは完成したBest Practiceではありません。Ideas / ODDの開発中に実際に起きたFailureから切り出した、最小のFork候補です。

## 1. 作ったAIにそのままレビューさせたら、レビューが作者寄りになった

制作中の意図や判断を知っているAIは、そのContextに引っ張られることがありました。

**Minimum Fork:** [`fresh-review/`](./fresh-review/)

制作途中の全会話や、作者側の長い説明は原則として渡しません。

ただし、Fresh Reviewは「何も知らないレビュー」ではありません。

制作過程の文脈は切りつつ、評価に必要な最新情報は渡します。

> Fresh context does not mean missing context.

まず1回、いつもの制作Sessionとは別のSessionでレビューして、論点の出方が変わるか観察してみてください。

Related: AI Product Team / Handoff

## 2. AIが質問しすぎて、探索がインタビューになった

何を話しても質問が返り、人間がずっと答える側になりました。

そこで質問を減らす方向へ振ると、今度は必要な質問まで減りました。

**Minimum Fork:** [`question-loop/`](./question-loop/)

まずは、

> 質問をDefaultにしない。必要なら質問する。質問以外の関わり方も選ぶ。

という小さい変更だけを試します。

目的は「質問を減らすこと」ではありません。

質問、観察、仮説、違いの提示、何もしない、といった関わり方を状況に応じて選べるかを見るためのExperimentです。

Related: Co-Explorer

## 3. 良いと思ったルールを守ったら、実際の体験が悪くなった

Ruleに沿っているのに、実際に使ってみると不自然になることがありました。

**Minimum Fork:** [`rule-vs-reality/`](./rule-vs-reality/)

Ruleをすぐ修正したり追加したりする前に、まず1件だけ、

- 実際に何が起きたか
- 何を期待していたか
- どこに違和感があったか
- どのRuleが関係していたか

を記録します。

Rule違反を直すのではなく、**Rule側が間違っている可能性も残す**ための最小構成です。

Related: Observation to Design / Reality First

## 4. 過去の判断をAIが現在にも適用し続けた

以前は妥当だった判断が、状況が変わったあとも現在の方針として扱われやすくなることがありました。

**Minimum Fork:** [`current-vs-past/`](./current-vs-past/)

最初はKnowledgeを細かく分類する必要はありません。

まず、

- 今の判断に使うもの
- 残しておくが、自動では現在の判断に使わないもの

だけを分けます。

必要なら各項目に、

```text
Status: Current / Hypothesis / Legacy