# 豆寄席 プレゼンテーション Constitution

## Core Principles

### I. Presentation Format
Marp Markdown形式でスライドを作成する。
クリーンでシンプルな構造を保ち、1スライドにつき1メッセージを徹底し、オンラインでも視認性の高いスライドを心がける。

### II. Visual Design & Theme
告知用画像（`images/title.png`）と世界観やトンマナを統一する。
- **デザインシステム:** GitHub標準である **Primer CSS** をベースとしたクリーンなデザインとし、アイコンには **Octicons** を活用する。
- **ベースカラー:** 会社のイメージカラーである **薄い紫色（ライトパープル）** を背景色などのベーストーンとする。
- **タイトルスライド:** `images/title.png` をベースにレイアウトする。
- **ロゴの配置:** 各スライドの右上に会社ロゴ（`images/mamezou.png`）を固定で表示する。
- **フッター要素:** フッターにはページ番号（スライド番号）のみを記載する。イベント名などのテキストは配置しない。

### III. Typography
オンラインの画面越しでも視認性の高い、可読性の高いサンセリフ体（ゴシック体）を採用する。
Primer CSS のタイポグラフィに準拠しつつ、日本語環境で読みやすいフォントを設定する。
- **メインフォント:** Primer の推奨するシステムゴシック（`-apple-system, BlinkMacSystemFont, "Segoe UI", ...`）をベースとし、日本語は `Noto Sans JP` など視認性の高いものにする。
- **フォントサイズ:** 見出しは太字で大きく、本文の多くは `24pt` 程度を基本としつつ、文字量が多い場面では最低 `20pt` までの縮小を許容する。
- **行間 / 余白:** Primer CSS のSpacingを意識し、十分な余白をとる。

### IV. Slide Layout & Marp Definitions
Marpでのスライドデザインでは、以下のCSS定義を基本方針とする。

```css
/* ロゴの右上固定配置の例 */
header {
  position: absolute;
  top: 20px;
  right: 30px; /* 位置はプレビューを見て微調整 */
  width: 120px;
  height: 40px;
  background-image: url('images/mamezou.png');
  background-size: contain;
  background-repeat: no-repeat;
  background-position: right top;
}

/* 背景色（薄い紫色） */
section {
  background-color: #F6F3FB; /* 薄い紫色の例（後ほど調整可） */
}
```
※ ページ番号は Marp のディレクティブ `<!-- paginate: true -->` を使用する。

## Workflow
- スライドの構成・原稿はまずMarkdownのテキストとして作成・推敲する。
- デザインの調整やOcticons・画像のレイアウトは、Marpのプレビューで確認しながら進める。
- Primer CSS のコンポーネントライクなスタイル（バッジやアラートなど）が必要な場合は、MarpのカスタムCSSで再現する。

**Version**: 1.1.0 | **Ratified**: 2026-03-05
