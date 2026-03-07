---
marp: true
theme: mamezou-theme
header: " "
---
<!-- class: title-slide -->
<!-- paginate: skip -->

![bg](../images/title.png)

---
<!-- class: "" -->
<!-- paginate: true -->

## 本日のゴール

皆さんのチームでは、AIを開発者の生産性向上のためだけに使っていませんか？

本日は、スクラムマスターがAIを活用することで、スクラムの三本柱をどのように強化できるか、プロジェクトでの実践内容をご紹介します。

- <strong>透明性の強化</strong>（AIを活用した指標の可視化）
- <strong>検査・適応の促進</strong>（AIによる第三者評価）

---

## 0. 自己紹介

<div class="two-columns">
<div>

<strong>石田朗大（あきひろ） 41歳</strong>

2023年10月 豆蔵入社
ビジネスソリューション事業部 
アジャイルグループ

前職（小売業ユーザー企業）でスクラムに出会い、本格的にその道に進みたいと決意し、豆蔵に入社しました。

</div>
<div class="rounded-image" style="text-align: center;">

![width:100%](../images/profile.jpg)

</div>
</div>

---

## 職務経歴
- <strong>2009.4 - 2017.3 独立系SIer</strong>
  - ウォーターフォール型での金融システム開発
- <strong>2017.4 - 2023.9 小売業 社内SE</strong>
  - 基幹システムの運用保守、刷新プロジェクト
- <strong>2023.10 - 現在 豆蔵 アジャイルグループ</strong>
  - 専任スクラムマスターとしてプロジェクトを支援

---

## 特技・趣味

<strong>ルービックキューブ</strong>

- 最少手数競技 アジア大会2014 3位
- メガミンクス シニア（40歳以上） 世界記録保持者
- 目隠しで揃えるための基本解法を日本に普及

---

## 最少手数競技

<div class="two-columns">
<div>

- ルービックキューブを<strong>どれだけ少ない手数で揃えられるか</strong>
- 制限時間は1時間。じっくりと考えて答えを導き出す。
- アジア大会入賞時（2014年）の記録は<strong>31手</strong>
- 今の世界記録は<strong>16手</strong>

</div>
<div class="rounded-image" style="text-align: center;">

![width:100%](../images/fmc.png)

</div>

---

## メガミンクス

<div class="two-columns">
<div>

- 正十二面体の形をした立体パズル
- 普通のルービックキューブより面が多く複雑
- シニア部門（40歳以上）
  世界記録保持者：平均 <strong>1:02.91</strong>

</div>
<div class="rounded-image" style="text-align: center;">

![width:100%](../images/megaminx_competition.png)

</div>
</div>

<div class="center-image">

![](../images/senior_rankings.png)

</div>

---

## 今回の豆寄席について

私は元々開発エンジニアでしたが、現在は専任のスクラムマスターとして動いています。

- 生成AIが急激に進化し、コードを書く「開発者」の生産性を劇的に向上させています。
- では、コードを書かない「スクラムマスター」はどうAIを使うべきか？

この課題について、実際に私が現場で実践している内容をご紹介します。

---
<!-- class: title-slide -->

# 第1部：スクラムとAIの導入
## スクラムガイド拡張パックから読み解く

---
<!-- class: "" -->

## スクラムガイド拡張パックとAI

2025年6月に公開された「[スクラムガイド拡張パック](https://scrumexpansion.org/ja/scrum-guide-expansion-pack/2025.6/)」では、人工知能（AI）がスクラムの実践を強化する重要な要素として定義されています。

---

## AIによるスクラムの強化領域

> <strong>AIは以下を通じてスクラムを強化する可能性がある：</strong>

<div class="small-list">

- <span class="Label">経験的プロセス制御</span>：AI駆動の分析により、透明性・検査・適応が改善される。
- <span class="Label">認知的拡張</span>：AIにより、人間のスクラムチームメンバーは戦略的・創造的・倫理的な検討に集中できる。
- <span class="Label">継続的な価値適応</span>：AIは、リアルタイムのユーザーフィードバックとトレンドに基づき、プロダクトバックログアイテムの更新と再優先順位付けを行うことができる。
- <span class="Label">システム洞察</span>：AIは隠れた相互依存関係を特定し、データに基づいた意思決定を改善する。

</div>

---

## 本日のフォーカス

本日は前記の4領域から、<strong>「経験的プロセス制御」</strong>にフォーカスします。

<strong>AI駆動の分析により、透明性・検査・適応が改善される。</strong>

スクラムの三本柱である「透明性・検査・適応」をAIでいかに強力に支援できるか、その実践事例をご紹介します。

---

## スクラムマスターとAIの役割分担 (1/2)

スクラムガイド拡張パックには、ユニークな一文が記載されています。

> <strong>The Scrum Master must be human.</strong>
> <strong>（スクラムマスターは人間でなければならない）</strong>

- チームとの協働や複雑な人間関係の調整といった、<strong>「人間にしか果たせない役割」</strong>の重要性への示唆。

---

## スクラムマスターとAIの役割分担 (2/2)

- AIはスクラムマスターを代替するものではなく、能力を拡張する<strong>「強力なパートナー」</strong>。
- 人間はより本質的な課題解決に集中し、データ分析や客観的評価といったタスクをAIに任せるという役割分担が鍵。

---
