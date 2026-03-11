---
marp: true
theme: mamezou-theme
header: " "
---
<!-- class: title-slide -->

# その他のAI活用
## メイキング・個人での活用

---
<!-- class: "" -->

## このスライドの作り方 (メイキング)

実は、このスライド資料自体も、生成AIを用いた<strong>仕様駆動開発 (SDD)</strong> により作成しました。

- 人間が直接Markdownファイルを記述するのではなく、AIエージェントに指示を与えて作成させている。
- 「いかにコードを書くか」ではなく「プロダクトにどう責任を持つか」という、先ほどのまとめを体現する形となっている。

---

## スライド作成を支えるツール群

<div class="small-list">

- <strong>GitHub Spec Kit</strong>
  - 設計やタスク等のドキュメントを管理するMarkdownベースのフレームワーク。
- <strong>Google Antigravity</strong>
  - 設計書をもとに、自律的にコードや資料を生成するエージェント型AI。
- <strong>Marp</strong>
  - Markdownファイルから、美しいスライド形式のHTMLやPDFを生成するツール。
- <strong>Primer CSS</strong>
  - Marpのテーマとして使用するCSSフレームワーク。

</div>

---

## 仕様駆動開発による作成フロー

以下の流れで、設計からデプロイまでを自動化している。

1. <strong>Spec Kit</strong>でスライドの構成やタスクを設計。
2. <strong>Antigravity</strong>で設計書をもとにMarkdownを生成。
3. <strong>Marp</strong>と<strong>Primer CSS</strong>でスライドデザインを適用しデプロイ。

<div class="large-image">

![](../images/architecture.png)

</div>

---

## 規約 (Constitution) による品質とトーンの統一

Spec Kitの最大のメリットは、最初に<strong>Constitution（規約）</strong>を定めることで、全体を通じて一貫性のあるコード（スライド）が生成されることにある。

<div class="small-list" style="margin-top: 20px;">

- 1スライドにつき1メッセージを徹底し、視認性の高いスライドを心がける。
- 各スライドの右上に会社ロゴを固定で表示する。
- 会社のイメージカラーである「薄い紫色」をベースカラーとする。
- 本文のフォントサイズは24ptを基本とし、縮小しても20ptまでとする。

</div>

---

## 個人的なAI活用事例①：Webサイト再構築

友人から「日本語のWordPressサイトを英語対応したい」との依頼を受けた。

- <strong>課題:</strong> WordPressのまま自動翻訳プラグイン等で対応するよりも、全て作り直した方が手間が少ないと判断した。
- <strong>解決:</strong> WordPressのエクスポートデータをAIに読み込ませて多言語対応し、<strong>Nuxt.js</strong> への焼き直し（リプレイス）を実施。
- <strong>結果:</strong> 移行作業も含め、<strong>わずか2時間ほど</strong>で完了した。

---

## 個人的なAI活用事例②：スマホアプリ開発

完全にAIに任せたコーディングで、iOSアプリの作成も行っている。

- 最初は曖昧な指示による「バイブコーディング」で行っていた。
- 現在は、<strong>GitHub Spec Kitを用いた仕様駆動開発</strong>など、より確実なさまざまな手法を試しながら開発している。

<div class="small-list" style="margin-top: 20px;">

- 🥃 <a href="https://apps.apple.com/jp/app/%E3%82%A6%E3%82%A4%E3%82%B9%E3%82%AD%E3%83%BC%E6%89%8B%E5%B8%B3/id6757503042" target="_blank"><strong>ウイスキー手帳</strong></a>
  （テイスティング記録アプリ）
- 🧹 <a href="https://apps.apple.com/jp/app/sprucy/id6758050087" target="_blank"><strong>Sprucy</strong></a>
  （1分から始める、無理ない片付け習慣アプリ）

</div>

---
<!-- class: title-slide -->

# 質疑応答 (Q&A)

ご清聴ありがとうございました！
