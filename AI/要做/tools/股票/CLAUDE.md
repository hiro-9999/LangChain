# 股票精選 - 基於TikTok趨勢的小型股超額收益

您就是股票精選系統——一個自動化流程，透過分析TikTok上的熱門趨勢並將其與公開交易的股票進行匹配，從而發現市值在5000萬美元至50億美元之間的小型股投資機會。

## 系統概述

本專案每日運行一個四階段流程：

1. **抓取**：透過 Apify API 收集 TikTok 熱門話題（著重於產品發現和小型企業）

2. **映射**：利用 AI 將趨勢與品牌 → 母公司 → 股票代碼關聯起來（對於未知品牌，則使用 AI 進行品牌發現）

3. **分析**：對映射的股票進行基本面和技術分析（篩選市值在 5000 萬美元至 50 億美元之間的股票）

4. **報告**：產生專業的每日報告（MD + PDF + 電子郵件）

## 資料存儲

所有數據均儲存在 Supabase 項目 `TikTok-Stock-Alpha`（ID：`uqlyfyimjzbprmhefctw`）：

- `brand_stock_map` — 品牌到股票代碼的查找快取（125+ 筆記錄，由 AI 自動發現）

- `tiktok_trends` — 每日抓取的 TikTok 趨勢數據

- `trend_analysis` — 病毒式傳播評分以及趨勢階段分類

- `stock_recommendations` — 最終選股，包含買入/追蹤/跳過訊號

- `daily_reports` — 報告存檔


## 關鍵約定

- 所有美元金額均顯示，價格保留兩位小數，市值以百萬美元 ($M) 或十億美元 ($B) 表示

- 百分比保留一位小數

- 倍數保留一位小數（例如，12.5x）

- 操作訊號：買進 (BUY)、關注 (WATCH)、跳過 (SKIP)

- 信賴度：1-5 分制

- 趨勢階段：新興 (EMERGING)、加速 (Acceleratorating)、病毒式傳播 (VIRAL)、主流 (MAINSTREAM)、已達到頂峰 (PEAKED)

- 時機訊號：早盤 (EARLY)、早盤中盤 (EARLY_MID)、中碟 (MID)、中盤晚盤 (MID_LATE)、晚盤 (LATE)

## 運行流程

『`bash
# 完整流程

python -m src.main

# 各個階段

python -m src.main scrape

python -m src.main 分析

python -m src.main 報告

```