---
marp: true
theme: default
paginate: false
size: 16:9
---

<style>
section { padding: 0; font-family: "Noto Sans JP", "Helvetica Neue", Helvetica, Arial, sans-serif; }

/* 上の大きなグレー領域 */
.hero {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  height: 70vh;
  background: #f5f5f5;
  text-align: center;
  box-sizing: border-box;
  padding: 2.5rem 2rem;
  border: 1px solid rgba(0,0,0,0.05);
  position: absolute;
  width: 100%;
  top: 0;
}

/* タイトル */
.hero h1 {
  margin: 0;
  line-height: 1.25;
  font-size: 2.3rem;  /* 小さめに調整 */
  font-weight: 800;
  color: #111;
  letter-spacing: -0.01em;
}

/* サブタイトル */
.hero p.subtitle {
  margin-top: 1.4rem;
  font-size: 1.1rem;
  color: #888;  /* 薄めグレー */
  font-weight: 500;
}

/* フッター領域 */
.footer {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  padding: 0.6rem 1.8rem;
  background: #fff;
  box-sizing: border-box;
  border-top: 1px solid rgba(0,0,0,0.05);

  position: absolute;
  width: 100%;
  bottom: 0;
}

/* 左の情報 */
.footer .meta {
  display: flex;
  flex-direction: column;
  gap: 0.25rem;
  font-size: 0.82rem;
  color: #444;
}

/* サブテキスト */
.footer .meta .sub {
  font-size: 0.72rem;
  color: #999;
}

/* ロゴ部分 */
.footer .logo {
  margin-top: 0.65rem;
  font-weight: 700;
  font-size: 0.78rem;
  color: #111;
}

/* CONFIDENTIALタグ */
.confidential {
  border-radius: 999px;
  padding: 0.2rem 0.6rem;
  font-size: 0.65rem;
  color: #e60012;
  border: 1px solid rgba(230,0,18,0.4);
  background: rgba(230,0,18,0.02);
  font-weight: 700;
  letter-spacing: 0.06em;
  align-self: flex-end;
  margin-bottom: 0.2rem; /* 下寄せ */
}
</style>

<section>
  <div class="hero">
    <h1>ここに資料のタイトルを<br>入力してください</h1>
    <p class="subtitle">サブタイトルが入ります</p>
  </div>

  <div class="footer">
    <div>
      <div class="meta">
        <div>名前や所属など</div>
        <div class="sub">日付やバージョンなど</div>
      </div>
      <div class="logo">DMM Group</div>
    </div>
    <div class="confidential">CONFIDENTIAL</div>
  </div>
</section>
