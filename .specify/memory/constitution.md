# 豆寄席 プレゼンテーション Constitution

## Core Principles

### I. Presentation Format
Marp Markdown形式でスライドを作成する。
クリーンでシンプルな構造を保ち、1スライドにつき1メッセージを徹底し、オンラインでも視認性の高いスライドを心がける。

### II. Visual Design & Theme
告知用画像（`images/title.png`）と世界観やトンマナを統一する。
- **デザインシステム:** GitHub標準である **Primer CSS** をベースとしたクリーンなデザインとし、アイコンには **Octicons** を活用する。
- **ベースカラー:** 会社のイメージカラーである **薄い紫色（ライトパープル）** を背景色などのベーストーンとする。
- **タイトルスライド:** 各章の表紙となるスライドは、**ダークパープル系のグラデーション**を背景色とし、リッチな印象を与える。また、元の白色の会社ロゴをそのまま白で表示する。
- **アイキャッチスライド:** 背景やアウトカムなど、通常のスライドとメリハリをつけて強調したいページには、**通常より少し濃い紫色のグラデーション**を背景色として適用する。
- **ロゴの配置:** 各スライドの右上に会社ロゴ（`images/mamezo.png`）を固定で表示する。元が白色のロゴのため、通常スライドでは黒抜き（`filter: brightness(0)`）にして表示する。
- **フッター要素:** フッターにはページ番号（スライド番号）のみを記載する。イベント名などのテキストは配置しない。

### III. Typography
オンラインの画面越しでも視認性の高い、可読性の高いサンセリフ体（ゴシック体）を採用する。
Primer CSS のタイポグラフィに準拠しつつ、アクセシビリティ（視認性）を最優先としてユニバーサルデザインフォントを設定する。
- **メインフォント:** 遠くからでも画面越しでも文字が潰れずにハッキリと読み取れる `"BIZ UDPGothic"` をベースとし、フォールバックとしてシステムゴシック（`-apple-system`, 等）を指定する。
- **フォントサイズ:** 見出しは太字で大きく、本文の多くは `24pt` 程度を基本としつつ、文字量が多い場面では最低 `20pt` までの縮小を許容する。
- **行間 / 余白:** Primer CSS のSpacingを意識し、十分な余白をとる。

### IV. Slide Layout & Marp Definitions
Marpでのスライドデザインでは、テーマCSSファイル `presentation/mamezou-theme.css` に定義する。以下は基本方針。

```css
/* ヘッダーのロゴ配置（通常スライド用） */
header {
  position: absolute;
  top: 20px;
  right: 30px;
  width: 120px;
  height: 40px;
  background-image: url('../images/mamezo.png');
  background-size: contain;
  background-repeat: no-repeat;
  background-position: right top;
  /* 元が白色のロゴのため、通常スライドでは黒抜きにして表示する */
  filter: brightness(0);
  opacity: 0.8;
}

/* 背景色（少し濃い紫色） */
section {
  background-color: #EDE1F8;
}
```
※ ページ番号は Marp のディレクティブ `<!-- paginate: true -->` を使用する。

### V. Utility Classes
スライド内で使用するユーティリティCSSクラスは以下の通り。

- **`.small-list`**: 箇条書きのフォントサイズを縮小し、情報量の多いスライドに使用する。
- **`.large-image`**: 画像を横幅いっぱいに表示しつつ、スライド下部から見切れないように高さを制限する。
- **`.center-image`**: 画像を中央寄せで60%幅に縮小表示する。
- **`.two-columns`**: スライド内容を左右2カラムに分割する。
- **`.rounded-image`**: 画像に角丸を適用して柔らかく見せる。
- **`.highlight-slide`**: スライド全体の色を薄いブルーに変更し、アイキャッチとして強調させる（`<!-- _class: highlight-slide -->`）。

### VI. Writing Style
- スライド本文の口調は **「だ・である」調（常体）** で統一する。
- ただし、導入パート（`00_intro.md`, `01_self_intro.md`）は聴衆への語りかけとなるため **「です・ます」調（敬体）** を使用する。
- 引用部分（`>`）は原文を尊重し、口調の統一対象外とする。
- 強調にはマークダウンの `**` ではなく、HTMLの `<strong>` タグを使用する（テーマCSSで色やスタイルが適用されるため）。

## Workflow
- スライドの構成・原稿はまずMarkdownのテキストとして作成・推敲する。
- テーマCSSファイルは `presentation/mamezou-theme.css` に配置する。
- デザインの調整やOcticons・画像のレイアウトは、Marpのプレビューで確認しながら進める。
- Primer CSS のコンポーネントライクなスタイル（バッジやアラートなど）が必要な場合は、MarpのカスタムCSSで再現する。
- Mermaid等の図は `images/src/` にソースコードを、`images/` に生成画像をそれぞれ管理する。

**Version**: 1.2.3 | **Ratified**: 2026-03-18
