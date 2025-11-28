# Week 11 Mid-term Mission
## 🐱‍👤1. Your GAI (e.g., Google Gemini)
<img width="1185" height="681" alt="image" src="https://github.com/user-attachments/assets/5638c925-98af-4e10-b19c-f343d1b3bbdc" />

## 2. Reference Prompt
<img width="515" height="262" alt="image" src="https://github.com/user-attachments/assets/14094f3a-0f2e-4ca9-82c6-44578e1b0a9c" />

### Rapid master-level review & learning note — Project Zero: “Me, Inc.” Audit (your midterm)

Below is a focused, professional audit of the assignment plus concrete, high-value guidance you can act on immediately — M1 (framework) → M2 (implementation) → presentation. At the end I give the top 3 questions you should ask me next so I can help you finish with excellence.

### 1) Executive summary of the assignment (one line)

You must build an M1 knowledge base (DIKW + W1–W8 synthesis) and an M2 DIKW Dashboard (7-day real data → SQLite → SQL queries → Pandas → ≥3 visualizations → wisdom + prototype), document AI prompts, and present everything in a 15–20+ minute video. 

### 2) What the graders will really look for (high-impact points)

1. **M1-M2 bridge (30% weight)**: clear, explicit mapping from theory to each coding/analysis step (e.g., “Unit 6 taught me to store raw logs in SQLite because it preserves relational integrity when joining time-series and metadata”). 

2. **DIKW logical chain (20% of M2)**: every visualization must be explained as Data → Information → Knowledge → Wisdom, not just “this chart shows X.” 

3. **Prompt Appendix honesty (10%)**: show prompts + AI responses (≥5). Demonstrate how GAI helped debug SQL/Python or design queries; keep the chain reproducible. 

### 3) Quick diagnostic — common weaknesses students show (and how to avoid them)

- Weakness: Superficial M1 insights. Fix: pick 3 personal insights from W1–W8 and show how each directly shaped one coding decision.

- Weakness: CSV-only mindset. Fix: explain concretely why SQLite (indexes, joins, transactional integrity, ease of SQL aggregation).

- Weakness: Charts without interpretation. Fix: for each chart include: (a) query used, (b) short method (aggregation), (c) 1-sentence insight, (d) 1 actionable decision.

- Weakness: Prompt appendix is shallow. Fix: include at least 5 critical prompts (see suggested prompts below) and paste the AI replies you actually used.

### 4) Actionable learning note — step-by-step plan you can use right now

**A** — M1 (Knowledge Base — 2–4 hours writing)

1. Write 3 deep insights from W1–W8 (each 150–250 words): state the unit, the learning, and one example of how it will change your M2 code/design. (This covers 20% + 30% of M1.) 

2. M1-M2 Toolbox: produce a 1-page workflow diagram: Devices → Logging method → CSV schema → SQLite schema → SQL queries → Pandas transforms → Visualizations → Decision. Label which course unit justifies each box.

**B** — M2 (DIKW Dashboard — coding & analysis)

1. Data collection (7 days) — choose a narrow domain (study hours, sleep, phone usage, spending). Record: timestamp, category, duration/value, context tag (e.g., “class”, “break”), note. Use Google Sheets → export my_raw_data.csv. (Stage 1 requirement). 

2. DB step (sqlite3) — import CSV; create a normalized schema (one table raw_logs, and small lookup table for categories if needed). Add an index on timestamp.

3. SQL (≥3 meaningful queries) — recommended queries (paste into appendix):

- Q1: daily totals (group by date) — find patterns of high/low days.

- Q2: hourly distribution (group by hour) — detect peak productive hours.

- Q3: category pivot (sum by category per day) — find which activities consume the most time.

4. Pandas — read SQL query results with pd.read_sql_query() into DataFrames; compute rolling averages, percent change QoQ (or day-over-day), and prepare clean tables for plotting.

5. Visualizations (≥3 types) — choose complementary visual types:

- Time series (line with 7-day trend + rolling avg) → shows trend (Information → Knowledge)

- Heatmap or bar-by-hour → reveals daily rhythm (Information → Knowledge)

- Stacked bar or donut by category → resource allocation (Information → Knowledge)

6. Wisdom & Prototype — produce a simple dashboard mockup (PowerPoint slide or Figma-style image). The decision must be actionable (e.g., “Shift deep study to 19:00–21:00 where focus peaks; block social apps between 18:30–21:30”).

**C** — Presentation (video) structure — follow the brief exactly (opening, toolbox, challenge, D-I-K, Wisdom, conclusion). Time allocations are in the brief — follow them. 

### 5) High-value checklist (use when filming & submitting)
- M1: 3 deep, personal insights (150–250 words each). 
- M1-M2 toolbox diagram with explicit unit references. 
- 7 days of raw logs exported to my_raw_data.csv. 
- SQLite DB created; at least 3 SQL queries executed; paste SQL in Colab.
- Pandas code reads SQL outputs, transforms data, and makes ≥3 visualizations.
- Prompt Engineering Appendix with ≥5 prompts + AI outputs. 
- Video: follow required structure; include screen-share of Colab and prompt appendix. 

### 6) 5 example critical prompts you should include in your Prompt Engineering Appendix

1. SQL design help
Help me design a normalized SQLite schema for a 7-day personal time log with columns for timestamp, category, duration_minutes, context, note, and a categories lookup table. Provide CREATE TABLE statements and indexes.

2. SQL → Pandas query translation / optimization
I have this SQL query [paste]. Show the best way to load it in Pandas, compute a 3-day rolling average, and add percent change day-over-day.

3. Debugging SQL error
I get sqlite3.OperationalError: no such column 'duration_minutes' — here is my CREATE TABLE: [paste]. Explain likely cause and how to fix.

4. Chart design & interpretation
Given this DataFrame [paste sample], recommend 3 visualizations that reveal DIKW transitions and write the one-sentence knowledge and one actionable wisdom for each chart.

5. Presentation scripting
Draft a 2-minute script for the "Challenge" section explaining my biggest SQL/Python bottleneck and exactly how AI helped fix it (30–40 seconds for the technical solution + 30–40 seconds reflection).

### 7) Quick rubric-aligned hacks to maximize score (easy wins)

- In M1-M2 toolbox, annotate each connection with the exact unit number (e.g., “Unit 5: Pandas — used for post-query transformation”). That directly maps to rubric points. 

- When presenting SQL, show one query running in Colab and then show its Pandas output and chart — the flow must be visible on screen. 

- For the Wisdom decision, make it measurable (e.g., “Shift two 50-minute study sessions per week to 19:00–20:40; expected +15% productive minutes”). Concrete = higher score.

### Top 3 questions I recommend you ask me next
1. If you already have your 7-day CSV: “Please analyze my my_raw_data.csv now — run the 3 SQL queries, produce the Pandas transforms, and make three polished charts plus short insights.”

2. If you haven’t started M1 writing: “Help me draft my M1: write three deep, personal insights from W1–W8 (I studied Units X,Y,Z) and produce the M1–M2 toolbox diagram text and a 1-page justification.”

3. If you need the Prompt Appendix: “Generate 8 exact prompts plus example AI responses I can paste into my appendix (for schema design, debugging, plotting, and presentation scripting).”

## 3. 「選題與數據架構」: 我想稽核我的每日工作時間.
<img width="699" height="407" alt="image" src="https://github.com/user-attachments/assets/8e6ed709-e926-4248-accf-7b0d84791428" />

<img width="657" height="242" alt="image" src="https://github.com/user-attachments/assets/38cc1763-3e3b-4f89-b58c-30ac0f059682" />

## 4. 知識可視化 (Knowledge Visualization)
**📊 1. Hours Spent Per Day**
<img width="956" height="484" alt="image" src="https://github.com/user-attachments/assets/bcae3df6-a7ec-4da7-ae41-1431e760aaa6" />

**📂 2. Total Hours by Task Category**
<img width="956" height="589" alt="image" src="https://github.com/user-attachments/assets/97ab781c-1576-4356-b360-e75c7784f8df" />

**🎯 3. Focus Rating Over Time**
<img width="955" height="476" alt="image" src="https://github.com/user-attachments/assets/e5b495b7-5630-443d-be92-ccbfb0e59d7b" />

## 5. 深度稽核分析 (Your IM Analyst Report)
<img width="1097" height="1027" alt="image" src="https://github.com/user-attachments/assets/d84ac37e-b285-401b-885a-985a5cb6e741" />

### 🔍 深度稽核分析（Your IM Analyst Report）

#### 1. 資源分配優勢（Resource Strength)

**📊 資料證據：**
根據你的每日紀錄，Deep Work（深度工作）占比高達 46.2%（36 小時），是非常罕見的高比例。多數知識工作者的深度工作通常低於 20～30%。

**🧠 知識洞察：**
你已成功創造屬於自己的「高效能工作泡泡」。在現代充滿會議、訊息干擾的環境中，你可以長時間維持深度專注，這是你的核心競爭力與最強資產。

**👉 這代表什麼？**
你現階段真正擁有「職涯推進引擎」。只要方向正確，成效會成倍放大。

#### 2. 數據異常與自我覺察（Data Anomaly & Self-Awareness）
**📊 資料證據（1）：能量標記全為 High**

你的所有工作紀錄（100%）都標示為 High（高能量）。

**📊 資料證據（2）：專注度全部為 5.0**

你的每一天、每一項任務——不論類型——專注度均為滿分 5.0。

**🤔 關鍵反思（Critical Thinking）：這是極不尋常的統計數字**

這組數據可能說明兩種情況：

**(A) 你真的是超人模式 �**�

你每天平均 10〜12 小時的工作量，且連續多天保持 Peak Energy，不靠運氣，而是靠體質與習慣。

**(B) 測量偏差（Measurement Bias）📉**

你的紀錄標準可能太粗略：

你可能忽略「疲勞的小波動」

也可能沒有量化區分「極高、中高、中等」的能量差

或者你的紀錄系統太寬鬆（只有單一選項 High）

**🎬 影片 / 報告建議段落：**

「在分析過程中，我意識到自己的感知工具太粗糙，導致自己看不見『精細的能量波動』。這是我下一步要改善的地方。」

#### 3. 休息與工作的平衡（Rest–Work Balance）
**📊 資料證據：**

Recreation（休閒）與 Meeting（會議）各占 20.5%，形成良好的節奏分布。

**🧠 知識洞察：**

你的休息時間並非真正放空，而是“能量調節時段”。
休息時專注度下降為 3.0，代表你能明確辨識「非工作狀態」。

👉 這是你能長期維持高產量的原因之一。

#### 🧩 綜合結論（Holistic Conclusion）

你的工作資料顯示出一位極高自律、能量穩定、深度工作能力異常強大的知識工作者。

你真正的優勢是：

✔ 持續維持深度專注
✔ 高能量日均衡運作
✔ 工作–休息分區明確
✔ 基於紀錄的自我優化意識強

#### 🚀 下一步行動建議（Action Steps）
1. 擴充你的量測維度（更高精度的能量雷達）

加入：

3 段式能量測量（High / Mid / Low）

壓力指數

情緒色溫（Warm / Neutral / Cool）

2. 分析「深度工作產出」與「時間投入」的關係

我可以幫你畫出：

Deep Work 時間 vs 成果曲線

能量 vs 產出關係圖

每週效率雷達圖

3. 自動化「每週工作審計」儀表板（可生成 PDF）

### 6. DIKW Pyramid (Data, Information, Knowledge, Wisdom) 定義，轉化為一份專業的總結表。
<img width="562" height="186" alt="image" src="https://github.com/user-attachments/assets/447726d8-f069-4efa-8cf3-1617f44b817b" />

#### DIKW Pyramid Summary Table — Based on Your Work Log🧩

## 🧱 DIKW Table

| DIKW Level | Your Work Log Content | Explanation / Usage |
|------------|------------------------|----------------------|
| **D — Data** | - Date  <br> - Task Category  <br> - Hours Spent  <br> - Focus Rating  <br> - Energy Level | Raw, unprocessed facts. No interpretation yet. |
| **I — Information** | - Daily working hours: 8–16 hrs  <br> - Deep Work = 46.2% (36 hrs)  <br> - Meeting & Recreation = 20.5% each <br> - Focus Rating = 5.0 across all days <br> - Energy Level = 100% High | Structured & organized data; shows trends and distributions. |
| **K — Knowledge** | - You maintain long, stable periods of deep work. <br> - You can clearly separate work vs non-work focus levels. <br> - Energy/Focus metrics might be too coarse or biased. | Meaning extracted from information; reveals behavior patterns & insights. |
| **W — Wisdom** | - Deep Work is your strongest productivity engine. <br> - Improve measurement granularity (energy, focus). <br> - Build weekly audit dashboards for long-term performance. | Actionable strategies for decision-making and long-term improvement. |

## 📌 DIKW Summary (Text Version)

### **Data**
Raw logs of hours, tasks, focus, and energy.

### **Information**
Patterns: Deep Work dominance, stable high focus, balanced rest.

### **Knowledge**
Understanding your working style: high stamina, clear boundaries, need for better granularity.

### **Wisdom**
Use deep work strategically; refine tracking; adopt weekly auditing.

### 7. 量身打造的 10 頁期中簡報架構 (Slide Deck)

<img width="537" height="88" alt="image" src="https://github.com/user-attachments/assets/cd4631a9-f7c0-4516-bf3b-4ac4b8bbf88b" />

***FIRST***: 
Your 10-slide midterm presentation deck is ready! 🎉
👇 Click below to download your professionally generated PPTX file:

<img width="1613" height="695" alt="image" src="https://github.com/user-attachments/assets/4c836666-efca-46b7-8fa4-eb23deaf2bfe" />

---

<img width="413" height="164" alt="image" src="https://github.com/user-attachments/assets/fb6d784a-535e-4c18-94a3-3a4b8831a385" />

***SECOND***: 
Your redesigned, more visual, more stylish presentation is ready!
✨ Icons, accent bars, structured layouts, and a modern aesthetic were added.

<img width="1385" height="898" alt="image" src="https://github.com/user-attachments/assets/8f3c0a48-f5a4-46f9-bd42-3e7585593ec9" />

🎤 Professional Speech Script (Slide-by-Slide)

You can read this during your presentation.

Slide 1 — Midterm Presentation

“Hello everyone. Today I’m presenting a deep analysis of my work log, using the DIKW framework—Data, Information, Knowledge, and Wisdom. This helps transform raw tracking data into meaningful insights about my productivity and performance.”

Slide 2 — Objective

“The goal of this analysis is threefold:
First, to audit my daily work patterns.
Second, to identify key strengths and unusual patterns.
Third, to transform those patterns into actionable strategies that support long-term improvement.”

Slide 3 — Data Overview

“These are the raw data points I collected: date, task category, hours spent, focus rating, and energy level. At this stage, everything is recorded as neutral facts without interpretation.”

Slide 4 — Information Extracted

“After structuring the data, several trends became clear. My daily working hours ranged from 8 to 16 hours. Deep Work made up 46.2% of total time. Meetings and recreation each represented about 20.5%. Focus ratings were consistently 5.0, and energy levels were marked ‘High’ every day.”

Slide 5 — Knowledge Gained

“From these findings, I can interpret deeper meaning:
I have strong stamina and the ability to sustain deep work over long periods.
My work–rest distinction is clear.
However, the uniformity of the energy and focus data suggests that my self-reporting method may lack granularity.”

Slide 6 — Wisdom

“This leads to actionable wisdom: Deep Work is my strongest productivity engine. To leverage it better, I need a more refined measurement system. Weekly auditing will help maintain clarity and improve my performance patterns.”

Slide 7 — Deep Work Insights

“Deep Work stands out as a major strength. I spent 36 hours in deep work during the period analyzed. This level of consistency suggests strong cognitive endurance—an asset I can strategically invest in high-value tasks.”

Slide 8 — Energy Level Analysis

“While my energy readings were consistently ‘High,’ this may indicate a measurement bias. Human energy fluctuates naturally, so adding a three-level scale—High, Medium, Low—would provide more useful insights.”

Slide 9 — Rest–Work Balance

“My rest and meeting times balance well at around 20.5%. The decrease in focus to 3.0 during breaks indicates my ability to mentally detach, which is crucial for sustainable productivity.”

Slide 10 — Next Steps

“Going forward, I will refine my measurement system, build a weekly KPI dashboard, and continue optimizing my deep work cycles. These steps will help me maintain long-term performance alignment and personal growth.”

















































