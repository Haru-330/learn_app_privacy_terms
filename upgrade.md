---
layout: page
title: プラン機能のご紹介
permalink: /plan
---

<style>
      /* -------------------------

Colors from DicstaTheme
------------------------- \*/
:root {
--primary-blue: #2196f3;
--secondary-indigo: #7e7cff;
--accent-red: #ff6b81;
--on-primary-dark: #ffffff;
--background-light: #f7faff;
--on-background-light: #0d1524;
--surface-light: #ffffff;
--on-surface-light: #0d1524;
--surface-variant-light: #e4ecfa;
--on-surface-variant-light: #2e3c56;
--outline-blue: #2b3f62;
}

      /* -------------------------

Basic Reset
------------------------- \*/
body {
margin: 0;
font-family: Arial, sans-serif;
background-color: var(--background-light);
color: var(--on-background-light);
}

      /* -------------------------

Dialog Container
------------------------- \*/
.dialog {
position: fixed;
top: 0;
left: 0;
width: 100%;
height: 100%;
background-color: rgba(13, 21, 36, 0.5);
display: flex;
justify-content: center;
align-items: center;
overflow-y: auto;
padding: 20px;
box-sizing: border-box;
}

      .dialog-content {
        background-color: var(--surface-light);
        border-radius: 12px;
        width: 100%;
        max-width: 480px;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        padding: 20px;
        display: flex;
        flex-direction: column;
      }

      /* -------------------------

Header
------------------------- \*/
.dialog-header {
display: flex;
align-items: center;
justify-content: space-between;
height: 56px;
margin-bottom: 16px;
}

      .dialog-header h2 {
        font-size: 18px;
        font-weight: bold;
        text-align: center;
        flex: 1;
        margin: 0;
      }

      .icon-button {
        background: none;
        border: none;
        cursor: pointer;
        font-size: 20px;
      }

      /* -------------------------

Scrollable Content
------------------------- \*/
.dialog-body {
display: flex;
flex-direction: column;
gap: 18px;
overflow-y: auto;
}

      /* -------------------------

Feature Comparison Card
------------------------- \*/
.card {
background-color: var(--surface-light);
border-radius: 12px;
padding: 16px;
box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

      .card h3 {
        font-size: 16px;
        font-weight: 600;
        margin: 0 0 12px 0;
      }

      .feature-row {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 12px 0;
        border-bottom: 1px solid rgba(0, 0, 0, 0.1);
      }

      .feature-name {
        flex: 1;
        font-weight: 500;
      }

      .feature-status {
        flex: 1;
        text-align: center;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 6px;
      }

      .feature-status.enabled {
        color: var(--primary-blue);
      }

      .feature-status.disabled {
        color: var(--on-surface-variant-light);
      }

      /* -------------------------

Plan Cards
------------------------- \*/
.plan-card {
border-radius: 12px;
border: 1px solid var(--outline-blue);
padding: 14px;
display: flex;
flex-direction: column;
gap: 10px;
}

      .plan-title {
        display: flex;
        justify-content: space-between;
        align-items: center;
        font-weight: bold;
        font-size: 16px;
      }

      .recommended {
        background-color: var(--primary-blue);
        color: var(--on-primary-dark);
        padding: 2px 6px;
        border-radius: 8px;
        display: flex;
        align-items: center;
        gap: 4px;
        font-size: 12px;
      }

      .plan-price {
        font-size: 24px;
        font-weight: 800;
      }

      .plan-period {
        margin-left: 6px;
        font-size: 14px;
      }

      .plan-monthly {
        font-weight: 600;
        color: var(--primary-blue);
        margin-top: 4px;
      }

      .plan-features {
        display: flex;
        flex-direction: column;
        gap: 6px;
      }

      .plan-feature {
        display: flex;
        align-items: center;
        gap: 8px;
      }

      .check-icon {
        color: var(--primary-blue);
      }
      .close-icon {
        color: var(---accent-red);
      }

      /* -------------------------

Note
------------------------- \*/
.note {
text-align: center;
text-decoration: underline;
font-size: 12px;
color: var(--on-background-light);
margin-top: 8px;
}
/* -------------------------
Responsive (Mobile)
------------------------- */
@media (max-width: 480px) {
  .dialog {
    padding: 12px;
  }

  .dialog-content {
    max-width: 100%;
    border-radius: 10px;
    padding: 16px;
  }

  .dialog-header h2 {
    font-size: 16px;
  }

  .feature-row {
    flex-direction: column;
    align-items: flex-start;
    gap: 6px;
  }

  .feature-status {
    justify-content: flex-start;
  }

  .plan-price {
    font-size: 20px;
  }
}

</style>

<div class="dialog">
  <div class="dialog-content">
<!-- Header -->
<div class="dialog-header">
  <h2>プレミアム機能で制限を解除</h2>
  <div style="width: 24px"></div>
</div>

<!-- Scrollable Body -->
<div class="dialog-body">
  <!-- Feature Comparison Card -->
  <div class="card">
<h3>機能比較</h3>

<div class="feature-row">
  <span class="feature-name"></span>
  <span class="feature-status">無料プラン</span>
  <span class="feature-status enabled">プレミアム</span>
</div>

<div class="feature-row">
  <span class="feature-name">文字起こし回数</span>
  <span class="feature-status disabled"
><span class="close-icon">✕</span>1日3ファイルまで</span
  >
  <span class="feature-status enabled"
><span class="check-icon">✔</span>無制限</span
  >
</div>

<div class="feature-row">
  <span class="feature-name">教材作成数</span>
  <span class="feature-status disabled"
><span class="close-icon">✕</span>制限あり</span
  >
  <span class="feature-status enabled"
><span class="check-icon">✔</span>無制限</span
  >
</div>

<div class="feature-row">
  <span class="feature-name">広告表示</span>
  <span class="feature-status disabled"
><span class="close-icon">✕</span>あり</span
  >
  <span class="feature-status enabled"
><span class="check-icon">✔</span>なし</span
  >
</div>
  </div>

  <!-- Plan List Title -->
  <h3>プラン一覧</h3>

  <!-- Plan Cards -->
  <div class="plan-card">
<div class="plan-title">
  <span>1年プラン</span>
  <span class="recommended">⭐ おすすめ</span>
</div>
<div>
  <span class="plan-price">¥ 3,600</span
  ><span class="plan-period">/ 年</span>
  <div class="plan-monthly">月あたり ¥300</div>
</div>
<div class="plan-features">
  <div class="plan-feature">
<span class="check-icon">✔</span>広告の削除
  </div>
  <div class="plan-feature">
<span class="check-icon">✔</span>教材作成数が無制限
  </div>
  <div class="plan-feature">
<span class="check-icon">✔</span>文字起こしが無制限
  </div>
</div>
  </div>

  <div class="plan-card">
<div class="plan-title">
  <span>1ヶ月プラン</span>
  <span></span>
</div>
<div>
  <span class="plan-price">¥ 450</span
  ><span class="plan-period">/ 月</span>
</div>
<div class="plan-features">
  <div class="plan-feature">
<span class="check-icon">✔</span>広告の削除
  </div>
  <div class="plan-feature">
<span class="check-icon">✔</span>教材作成数が無制限
  </div>
  <div class="plan-feature">
<span class="check-icon">✔</span>文字起こしが無制限
  </div>
</div>
  </div>

  <div class="plan-card">
<div class="plan-title">
  <span>広告削除のみ</span>
  <span></span>
</div>
<div>
  <span class="plan-price">¥ 980 </span
  ><span class="plan-period">(買い切り)</span>
</div>
<div class="plan-features">
  <div class="plan-feature">
<span class="check-icon">✔</span>広告の削除
  </div>
</div>
  </div>

  <!-- Note -->
  <div class="note">
※プランを購入するには会員登録・ログインが必要です。
  </div>
</div>
<!-- dialog-body -->
  </div>
</div>
