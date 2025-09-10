---
marp: true
title: Marpで学ぶHTML/CSS
theme: mytheme
paginate: true
# header: 'Marpで学ぶHTML/CSS'
footer: 'Think Frontend #8'
---

<!-- _class : title -->
# Marpで学ぶHTML/CSS
## Think Frontend #8

合同会社DMM.com 戦略開発本部
平良昂也

---

<!-- _class : content1 -->
# 自己紹介

<div style="margin-top:6%;">
    <div style="display: flex; gap: 8px;">
        <h2 style="margin: 0;">平良 昂也</h2>
        <div>(@__ayanoYuki_)</div>
    </div>
    <ul>
        <li>合同会社DMM.com（2025新卒）
            <ul>
                <li>戦略開発本部 DMMTV開発部<br>Webアプリケーション開発グループ</li>
            </ul>
        </li>
        <li>DMM TVのバグ修正をしている</li>
    </ul>
</div>

<img src="./.image/My Icon001.jpg" width="350px" 
     style ="position: absolute; top:26%; right: 10%">

---

<!-- _class : content1 -->
# Marpとは

<h2 style="width:100%; text-align: center;"> Markdown でスライドを作れるツール </h2>

<div class="container" style="margin-top: 0px">
    <div class="column">
        <img src="./.image/github.png" width="200px" style="margin-bottom: 15px;">
        <div style="font-weight: bold; font-size: 30px;">
            Git管理・自動化できる
        </div>
    </div>
    <div class="column">
        <img src="./.image/vscode.png" width="200px" style="margin-bottom: 15px;">
        <div style="font-weight: bold; font-size: 30px;">
            エディタだけで作れる
        </div>
    </div>
    <div class="column">
        <img src="./.image/ai.png" width="200px" style="margin-bottom: 15px;">
        <div style="font-weight: bold; font-size: 30px;">
            生成AIと相性が良い
        </div>
    </div>
</div>

---

<!-- _class : content1 -->
# 他サービスとの比較

<!-- | ツール            | 入力形式       | 出力形式        | 特徴                                                                 | 学習コスト |
|-------------------|---------------|----------------|----------------------------------------------------------------------|------------|
| **Marp**          | Markdown      | HTML, PDF, PPTX | シンプルなMarkdown拡張でスライド作成可能。テーマやカスタムCSS対応。   | 低         |
| **Reveal.js**     | HTML, Markdown| HTML            | 高機能でWeb向け。インタラクティブ性やアニメーションが豊富。           | 中         |
| **Slidev**        | Markdown (Vue)| HTML, PDF       | Vueベース。コード埋め込みやライブデモ、開発者向け機能が充実。          | 中〜高     |
| **Pandoc + Beamer**| Markdown, LaTeX| PDF (LaTeX経由) | LaTeXの美しい組版を利用可能。カスタマイズ性は高いがやや難解。          | 高         | -->


| ツール        | 入力    | 学習コスト | テーマ |
|---------------|---------|------------|------------|
| Marp          | MD      | 低         | ○ (シンプル)    |
| Reveal.js     | MD/HTML |  中         | ◎ (豊富)        |
| Slidev        | MD(Vue) |  中〜高     | ◎ (自由度高)    |
| Pandoc+Beamer | MD/TeX  |  高         | △ (LaTeX依存)   |

---

<!-- _class : content1 -->
# HTML/CSS次第でデザインが無限大

<h2 style="width:100%; text-align: center;"> MarpはMarkdownなので、HTML/CSSが使える！ </h2>

| 技術     | 役割・用途                 |
|----------|----------------------------|
| Markdown | 基本的なレイアウトを設定する |
| CSS      | スライドのデザインを設定する |
| HTML     | 細かなレイアウトを設定する |

---

<!-- _class : content1 -->
# HTML/CSSの腕試し・練習に使えそう

<style>
.githubish {
  width: 400px;
  height: 400px;
  display: inline-grid;
  place-items: center;
  margin-left: auto;
  margin-right: auto;
  margin-top: 30px;
}
.github-mark { color: #0d1117; }
.github-mark .cat { fill: #ffffff; }

h1, div {
    position: relative; 
    z-index: 100;
}
</style>

<div class="githubish">
<svg class="github-mark" viewBox="0 0 1024 1024" width="100%" height="100%">
  <circle cx="512" cy="512" r="500" fill="currentColor" />
  <path class="cat" d="M512 200c-174 0-316 142-316 316 0 140 91 258 217 300 16 3 22-7 22-16 0-8 0-29-1-57-88 19-107-42-107-42-14-35-34-45-34-45-28-19 2-19 2-19 31 2 47 32 47 32 27 47 72 34 90 26 3-20 11-34 20-42-70-8-143-35-143-155 0-34 12-61 32-83-3-8-14-40 3-83 0 0 27-9 88 32 26-7 54-11 82-11s56 4 82 11c61-41 88-32 88-32 17 43 6 75 3 83 20 22 32 49 32 83 0 120-73 147-143 155 11 9 21 27 21 55 0 40-1 72-1 82 0 9 6 19 22 16 126-42 217-160 217-300 0-174-142-316-316-316z" />
</svg>
</div>

<img src="./.image/スクリーンショット 2025-09-02 235309.png" class="background-image" style="opacity: 0.3;">

---

<!-- _class : content1 -->
# HTML/CSSの腕試し・練習に使えそう

デフォルトのテーマ＋Markdown onlyでは、デザイン・レイアウトに限界がある

<div class="container" style="margin-top: 0px;">
    <div class="column">
        <img src="./.image/スクリーンショット (39).png" width="500px">
    </div>
    <div class="column">
        <img src="./.image/スクリーンショット (38).png" width="500px">
    </div>
</div>

<h2 class="text-underline" style="width:100%; text-align: center;">FEなら、いつものスライドと同じデザインは作れるのでは？</h2>

---

<!-- _class : content1 -->
# スライドを作ってみよう！
合同会社DMM.comのスライドの表紙を作ってみたので、解説します！

<div style="text-align:center; width:100%;">
  <img src="./.image/スクリーンショット 2025-09-07 233759.png" style="height:70%; margin-top:15px;">
</div>

---

<!-- _class : content1 -->

<img src="./.image/スクリーンショット (40).png"  class="background-image" style="opacity: 1;">

---

<!-- _class : content1 -->

<img src="./.image/スクリーンショット (41).png"  class="background-image" style="opacity: 1;">

---

<!-- _class : content1 -->

<img src="./.image/スクリーンショット (42).png"  class="background-image" style="opacity: 1;">

---

<!-- _class : content1 -->

<img src="./.image/スクリーンショット (43).png"  class="background-image" style="opacity: 1;">

---

<!-- _class : content1 -->

<img src="./.image/スクリーンショット (44).png"  class="background-image" style="opacity: 1;">

---

<!-- _class : content1 -->
# ハマりどころ

<h2 style="width:100%; text-align: center;">
    パワーポイント形式の出力が弱い<br>
    （出力後の編集は不要で見た目をそのままでPPTX出力がしたい）
</h2>

<br>

- 基本の出力形式が**PDF, HTMLだけ**しかない
  - .pptxの出力をするには、設定が必要
- 出力した.pptxの編集は出来るが、**デザインをそのまま再現できない**
  - Marp v4.1.0から出来るようになった
  - フォントの設定だったり、配置が崩れたり...

---

<!-- _class : content1 -->
# 解決策・工夫

<h2 style="width:100%; text-align: center;">
    PDF形式で出力し、pdf2pptxをする
</h2>

<br>

1. MarpでスライドをPDF出力する
2. PDFをページ毎の写真にして、PPTXに貼る
3. PPTXを出力する

<h2 class="framed" style="margin-top: 30px;">
  CI/CDやスクリプトで自動化すれば実用的
</h2>


---

<!-- _class : content1 -->
# まとめ

- MarpはMarkdownベース で手軽にスライドが作れる  
- HTML/CSSを駆使すればデザイン自由度は高く、腕試しにも最適  
- 課題はPPTX出力の弱さ → PDF変換 + 自動化で実用可能  
- 他サービスと比較しても、学習コストが低く導入しやすいのが強み  

<h2 class="framed" style="margin-top:20px;">
  「軽く作りたい」「コードで管理したい」なら Marp が最適！<br>
  MarpでHTML/CSSの腕試し（パワポ芸）をやってみよう
</h2>

---

<!-- _class : title -->

<div style="text-align: center; position: relative; z-index: 100;">
    <img src="./.image/fin.png" width="30%">
</div>

<img src="./.image/background137.webp" class="background-image">