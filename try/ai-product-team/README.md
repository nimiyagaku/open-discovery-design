# Minimum Fork — AI Product Team

AI Product Teamを全部再現する必要はありません。

最初は、**「作る」と「レビューする」を別のContextに分ける**だけで試せます。

## 起きたFailure

Ideasの開発では、制作中の意図や判断を知っているAIに、そのまま同じSessionでレビューを頼むと、作者側のContextに引っ張られることがありました。

これは「AIを複数人に見立てたい」から始めたわけではありません。

まず扱いたかったのは、**同じContextを持ったまま制作と評価を続けることによる偏り**でした。

## Minimum Fork

```text
ai-product-team/
├── BUILDER.md
└── REVIEWER.md
```

この2つだけで始められます。

### Builder

普段どおり制作します。目的、制約、過去の判断など、制作に必要なContextを持っていて構いません。

### Reviewer

制作とは別Sessionでレビューします。

制作途中の会話や作者の自己弁護は原則渡しません。一方で、レビューに必要な情報まで削る必要はありません。

**渡すもの**

- 最新の成果物
- 最新の関連ドキュメント
- レビュー目的
- 評価に必要な前提・制約

**原則として渡さないもの**

- 制作Sessionの全会話
- 「なぜこうしたか」という制作途中の長い説明
- Builder自身の自己評価
- 過去のReviewerの結論（独立した初見を見たい場合）

> Fresh Reviewは「何も知らないレビュー」ではありません。  
> 制作過程のContextは切りつつ、評価に必要な最新情報は渡します。

> Fresh context does not mean missing context.

## まず1回試す

1. 普段のSessionで何かを作る。
2. 新しいSessionを開く。
3. `REVIEWER.md` と、最新成果物・最新ドキュメント・レビュー目的だけを渡す。
4. 「良くなったか」より、**論点の出方が変わったか**を見る。
5. 必要なら制作Sessionへ戻して判断する。

Reviewerの指摘が自動的に正しいわけではありません。Contextを分けても、独立した外部視点が生まれるとは限りません。

## うまくいったら増やす

2 Roleで価値があった場合だけ、必要に応じてRoleを増やします。

- **Meta-Reviewer** — Reviewの観点やRule自体を疑う
- **Specialist** — 特定領域だけ深く見る
- **Support** — 最適化とは別の認知位置を作る

最初からTeam全体を作る必要はありません。

## Related

- `practices/ai-product-team.md`
- `practices/handoff.md`

AI Product Teamの中心は、Role数ではなく**Contextと認知位置の分離**です。
