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

<h2 class="text-underline-pink" style="width:100%; text-align: center;">FEなら、いつものスライドと同じデザインは作れるのでは？</h2>

---

<!-- _class : content1 -->
# 実装してみた
今回は、DMMが使っているスライドデザインを再現してみます。



---

<!-- _class : content1 -->
# ハマりどころ

<h2 style="width:100%; text-align: center;">
    パワーポイント形式の出力が弱い<br>
    （基本出力形式と比較すると、出力後の手間がかかる）
</h2>

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

<img src="./.image/psd2pptx.svg" width="900px" style="margin-top: 30px; margin-left: auto; margin-right: auto;">

---

<!-- _class : content1 -->
# 他サービスとの比較

---

<!-- _class : content1 -->
# まとめ

---

<!-- _class : title -->
# Fin