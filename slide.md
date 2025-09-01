---
marp: true
title: Marpで学ぶCSS/HTML
theme: mytheme
paginate: true
# header: 'Marpで学ぶCSS/HTML'
footer: 'Think Frontend #8'
---

<!-- _class : title -->
# Marpで学ぶCSS/HTML
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
# CSS/HTML次第でデザインが無限大

<h2 style="width:100%; text-align: center;"> MarpはMarkdownなので、HTML/CSSが使える！ </h2>

| 技術     | 役割・用途                 |
|----------|----------------------------|
| Markdown | 基本的なレイアウトを設定する |
| CSS      | スライドのデザインを設定する |
| HTML     | 細かなレイアウトを設定する |


---

<!-- _class : content1 -->
# CSS/HTMLの練習/腕試しに使えそう

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
# 実装してみた
今回は、DMMが使っているスライドデザインを再現してみます。



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
# まとめ

- MarpはMarkdownベース で手軽にスライドが作れる  
- CSS/HTMLを駆使すればデザイン自由度は高く、腕試しにも最適  
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

<img src="./.image/background137.webp" 
    style="
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    border-radius: 20px;  
    width: 1200px;    
    height: 641px;
    z-index: 1;
    opacity: 0.6;  
">