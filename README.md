<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>乳房影像擴大月會暨介入實作課程</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: "Microsoft JhengHei", sans-serif;
      background: url('background.jpg') no-repeat center top;
      background-size: cover;
    }
    .poster {
      max-width: 1100px;
      width: 90%;      
      margin: 60px auto 0 auto;
      padding: 40px;
    }

/* Header Flex: logo 跨两行 */
.header-flex-two {
  display: flex;         /* 改成區塊 flex，而不是 inline-flex */
  width: 100%;  
  align-items: flex-start;    /* Logo 与两行文字顶部对齐 */
  justify-content: center;
  gap: 0px;           /*與右方文字標題留空格 */
  margin-bottom: 10px; /*與下方主題留空格 */
  text-align: center;
}

/* 调整 Logo 高度，使之约等于两行文字高度之和 */
.logo-two {
  height: 9em;  /* 约等于 2 × 1.8em 行高，可根据视觉微调 */
  object-fit: contain;
}

   /* 中文主标题 */
   .title-cn {
      display: flex; 
      justify-content: center;        /* 水平置中排列 */ 
      font-size: 2.6em;
      font-weight: bold;
      color: #2a5d70;
      line-height: 1.7;
      /* 如果你要限制最大寬度，也可以加上 max-width */
    }
     .title-cn span {
      flex: 1;
      text-align: center;
      font-size: 4em;        /* 跟 .year 保持一致 */
      color: #2a5d70;        /* 原本標題顏色 */
      line-height: 1;
      font-weight: bold;
     }

  /* 英文副标题 */
   .subtitle-en,
   .subtitle-en2 {
     font-size: 2.7em;
     line-height: 1;
     color: #007199;
     margin: 0;
     font-weight: 500;
     margin: 0px 0 0 0;         /* 上右下左 */
     text-align: left;
     flex: 0;
   }
   .subtitle-en  { text-indent: -2em; padding-left: 3em; }
   .subtitle-en2 { text-indent:  0;   padding-left: 0;   }


    .header {
      margin-top: 0px;
    }


    .full-width-divider {            /* 上下午課程間藍色細實線 */
      border: none;
      border-top: 2px solid #3399cc;
      width: calc(100% + 40px);      /* 彌補 section 的左右 padding 20px */
      margin: 24px -20px;
    
    }
    .topic-box {
      text-align: left;
      font-size: 2em;
      font-weight: bold;
      background: #2a5d70;
      color: white;
      padding: 12px 24px 12px 2em;
      border-radius: 12px;
      margin-top: 16px;
      margin-left: 0;
      width: 100%;
      box-sizing: border-box;
      line-height: 1.6;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
      display: inline-block;
    }
    .section {
      background: rgba(255, 255, 255, 0.8);
      box-sizing: border-box;
      width: 100%; 
      margin: 10px auto;
      border-left: 6px solid #3399cc;       /* 在區塊左側畫一條 6px 寬、實線、色碼 #3399cc（藍綠色）的邊框。 */
      padding: 20px;                        /* 內距四面都留 20px，讓內容（表格、文字）不會貼太近邊框， */
      border-top: 3px solid #99cce5;        /* 在區塊頂部加一條 1px 寬、實線、色碼 #99cce5（淺藍）的細邊框 */
      border-bottom: 1px solid #99cce5;
    }
    .section h3 {
      margin-top: 0;
      font-size: 1.7em;
      color: #005088;
    }
    .section table {
      width: 100%;

      border-collapse: collapse;
      font-size: 1.1em;
    }
    /* 時間欄位置中 */
    .section table th:nth-child(1),
    .section table td:nth-child(1) {
      text-align: center;
    }
    .section th,
    .section td {
      text-align: center;
      border: 1px solid #aad4e6;
      padding: 8px;
      background-color: white;

    }

    .bottom-box {
      display: grid;
      grid-template-columns: 1fr 1fr 205px;
      grid-template-rows: auto auto auto;
      background: #33a6cc;
    }
    .bottom-box .organizer-line,
    .bottom-box .contact {
      grid-column: 1 / span 2;
      background: rgba(255,255,255,0.8);
      padding: 12px;
      text-align: center;
      font-size: 1.1em;
      font-weight: bold;
      border-bottom: 1px solid #99cce5;
    }

.bottom-box .qr-wrapper {
  grid-column: 3;
  grid-row: 1 / span 3;
  /* 用 flex row，左右排列 */
  display: flex;
  align-items: center;      /* 垂直置中社群文字與圖 */
  justify-content: flex-end;/* 靠右對齊整個組 */
  gap: 0px;                /* 文字與圖之間留空 */
  padding: 0px 0px;           /* 左右各 8px 內距 */
}


/* 讓 qr-labels 裡的 span 直排 */
 .qr-wrapper .qr-labels {
  display: flex;
  flex-direction: column;
  align-items: center;
}

/* 保留原本的 qr-label 樣式 */
.qr-label {
  display: block;
  margin:  0;
  padding: 0px 10px;
  font-size: 1.8em;
  font-weight: bold;
  color: white;
  background: rgba(43,80,140,0.4);
  border-radius: 0px;
}

/* QR 圖片保持原本大小 */
.qr-image {
  width: 155px;
  height: auto;
  box-shadow: 0 2px 4px rgba(0,0,0,0.3);
}



</style>
</head>
      <body>
        <div class="poster">
          <div class="header-flex-two">
            <img src="logo.png" class="logo-two" alt="Logo"/>
            <div class="header-texts">
              <div class="title-cn">2025 南區月會擴大雙月會</div>
              <div class="title-cn">冰與火的微創：乳房消融技術臨床應用經驗分享</div>
          </div>
        </div>
    <div class="topic-box">
      上午主題｜乳房消融技術臨床應用經驗分享
    </div>
    
    <!-- ✅ 插入議程表區塊 -->
<div class="section">
  <h3>📅 上午課程</h3>
  <table>
  <colgroup>
    <col style="width: 13%;" />   <!-- 時間 -->
    <col style="width: 47%;" />   <!-- 議程主題 -->
    <col style="width: 40%;" />   <!-- 講者 / 單位 -->
  </colgroup>
    <thead><tr><th>時間</th><th>議程主題</th><th>講者 / 單位</th></tr></thead>
    <tbody>
      <tr><td>08:30–09:00</td><td colspan="2">報到</td></tr>
      <tr><td>09:00–09:30</td><td>冷凍與RFA在良性腫瘤微創治療之初步經驗</td><td>周春平 主任（高雄榮總）</td></tr>
      <tr><td>09:30–10:00</td><td>冷凍針與微創乳癌介入治療臨床應用</td><td>賴鴻文 主任（彰化基督教醫院）</td></tr>
      <tr><td>10:00–10:30</td><td>Coffee Time & 廠商介紹</td><td>                </td></tr>
      <tr><td>10:30–11:00</td><td>VABB with Mammotome</td><td>何蕙余 主任（仁愛長庚）</td></tr>
      <tr><td>11:00–11:30</td><td>RFA 治療早期乳癌之日本觀摩經驗分享</td><td>陳韋廷 醫師（高雄長庚）</td></tr>
      <tr><td>11:30–12:00</td><td>History and Clinical Practice of nonsurgical cryoablation for small breast cancer
 ( video lecture)</td><td>Dr. Eisuke Fukuma 主任（日本龜田）</td></tr>
      <tr><td>12:00–12:30</td><td>MAGNETIC RESONANCE IMAGING BEFORE AND AFTER BREAST CRYOSURGERY (Video lecture)   </td><td>Dr. Youichi Machida 主任（日本龜田）</td></tr>
      <tr><td>12:30–13:00</td><td colspan="2">午餐時間</td></tr>
    </tbody>
  </table>
</div>
 <!hr class="full-width-divider" />       <!-- 分隔線 --> 

 <div class="header">
      <div class="topic-box">下午主題｜乳房微創冷熱消融技術坊</div>
 

 <div class="section">
  <h3 style="margin-top:0px; margin-bottom:16px;">🛠 下午實作課程</h3>
  <table>
    <colgroup>
      <col style="width: 12%;" />   <!-- 時間 -->
      <col style="width: 47.9%;" />   <!-- 議程主題 -->
      <col style="width: 40.3%;" />   <!-- 講者 / 單位 -->
    </colgroup>
    <thead>
      <tr><th>時間</th><th>議程主題</th><th>講者 / 單位</th></tr>
    </thead>
    <tbody>
      <tr>
        <td>13:00–13:20</td>
        <td>乳房微創手術中護理</td>
        <td>吳雨蕎 護理師（高雄榮總）</td>
      </tr>
    </tbody>
  </table>


      <h3 style="margin-top:18px; margin-bottom:16px;">🔬 分站實作課程（13:20–15:20）</h3>
  <table>
    <colgroup>
      <col style="width: 10%;" />   <!-- 站別 -->
      <col style="width: 50%;" />   <!-- 主題內容 -->
      <col style="width: 25%;" />   <!-- 贊助單位 -->
      <col style="width: 15%;" />   <!-- 協助講師 -->
    </colgroup>
    <thead><tr><th>站別</th><th>主題內容</th><th>贊助單位</th><th>協助講師</th></tr></thead>
    <tbody>
      <tr><td>Station A</td><td>Cryotherapy</td><td>信裕公司、捷元生技公司</td><td>賴鴻文</td></tr>
      <tr><td>Station B</td><td>RFA</td><td>久立藥品有限公司</td><td>何蕙余</td></tr>
      <tr><td>Station C</td><td>VABB with Mammotome / Breast  ultrasound AI 實作</td><td>友信行醫療集團</td><td>陳韋廷</td></tr>
    </tbody>
  </table>
   <tr>
      <td colspan="3">
          <div style="font-size: 1.1em;margin-top:12px;">
             實作總協助講師：呂佳穎醫師、周春平醫師、洪振展醫師、吳雨蕎護理師
          </div>
      </td>
    </tr>
  </table>
</div>


<div class="bottom-box">
  <div class="organizer-line">主辦單位：財團法人王文浩放射線醫學基金會、高雄榮總放射線部</div>
  <div class="organizer-line">協辦單位：中華民國醫用超音波學會、中華民國放射線醫學會</div>
  <div class="contact">洽詢專線：0932-020091 Email：vghksbreast@gmail.com</div>

   <div class="qr-wrapper">
    <!-- 文字獨立包一層 -->
    <div class="qr-labels">
      <span class="qr-label">社</span>
      <span class="qr-label">群</span>
      <span class="qr-label">專</span>
      <span class="qr-label">區</span>
    </div>
    <!-- QR 圖放右邊 -->
    <img src="qrcode.png" alt="QR Code" class="qr-image" />
  </div>
</div>
</body>
</html>

