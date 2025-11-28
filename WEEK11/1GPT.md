# Week 11 Mid-term Mission
## 1. Your GAI (e.g., Google Gemini)
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
<img width="657" height="242" alt="image" src="https://github.com/user-attachments/assets/38cc1763-3e3b-4f89-b58c-30ac0f059682" />

## 4. 知識可視化 (Knowledge Visualization)
<img width="956" height="484" alt="image" src="https://github.com/user-attachments/assets/bcae3df6-a7ec-4da7-ae41-1431e760aaa6" />

<img width="956" height="589" alt="image" src="https://github.com/user-attachments/assets/97ab781c-1576-4356-b360-e75c7784f8df" />

<img width="955" height="476" alt="image" src="https://github.com/user-attachments/assets/e5b495b7-5630-443d-be92-ccbfb0e59d7b" />

## 5. 深度稽核分析 (Your IM Analyst Report)



























































