# Try one ODD failure

ODDを全部理解してから使う必要はありません。

下の中に「これ、自分のAI利用でも起きている」と思うものがあれば、そのケースだけ持っていって試してください。

ここにあるのは完成したBest Practiceではありません。Ideas / ODDの開発中に実際に起きた失敗から切り出した、最小のFork候補です。

## 1. AIが質問しすぎて、探索がインタビューになった

何を話しても質問が返り、人間がずっと答える側になりました。そこで質問を減らす方向へ振ると、今度は必要な質問まで減りました。

**Minimum Fork:** [`question-loop/`](./question-loop/)

まずは「質問をDefaultにしない。必要なら質問する。質問以外の関わり方も選ぶ」だけを試します。

Related: Co-Explorer

## 2. 作ったAIにそのままレビューさせたら、レビューが作者寄りになった

制作中の意図や判断を知っているAIは、そのContextに引っ張られることがありました。

**Minimum Fork:** [`fresh-review/`](./fresh-review/)

まずは制作Sessionとは別のSessionを作り、成果物・目的・必要な評価条件だけを渡してレビューします。

Related: AI Product Team / Handoff

## 3. 良いと思ったルールを守ったら、実際の体験が悪くなった

Ruleに沿っているのに、使ってみると不自然になることがありました。

**Minimum Fork:** [`rule-vs-reality/`](./rule-vs-reality/)

Ruleを直す前に「実際に何が起きたか」を1件だけ記録し、Rule側を疑う余地を残します。

Related: Observation to Design / Reality First

## 4. 過去の判断をAIが現在にも適用し続けた

以前は妥当だった判断が、状況が変わったあとも現在の方針として扱われやすくなりました。

**Minimum Fork:** [`current-vs-past/`](./current-vs-past/)

まずは「今の判断に使うもの」と「残しておくが自動では使わないもの」だけを分けます。

Related: Knowledge State Map / Handoff

## 5. 「なんでこうしたんだっけ？」をAIが綺麗なStoryで埋めた

記録は残っていても、意思決定時のContextが断片化していると、AIが自然な因果関係を補完することがあります。

**Minimum Fork:** [`decision-trace/`](./decision-trace/)

全部ではなく、間違って再利用されたときの影響が大きいDecisionだけ、元のObservationやSourceへ戻れる記録を残します。

Related: Handoff / Knowledge State / Reality First

---

## How to use

1. 今起きているFailureを1つ選ぶ。
2. そのFolderだけコピーする。
3. 普段のAI利用で一度試す。
4. 効いたかどうかより、何が変わったかを見る。
5. 理由を知りたくなったら、Related Concept / Practiceを読む。

ODD全体をForkする必要はありません。

> Take one useful difference. Leave the rest.
