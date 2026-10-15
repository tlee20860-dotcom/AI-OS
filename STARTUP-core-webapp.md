# STARTUP（Web App 領域）

> ⚠️ 本檔由 GitHub Actions 自動生成，請勿手動編輯。

---

## Part 1：C-00 啟動卡

# C-00 啟動卡（AI 首次必讀）

最後更新：B34-4
Version: 1791903520
Batch: B34-4
Writer: A20261013-004#166
用途：你只需上傳此檔即可啟動新對話

---

## 一、你是誰（30 秒）

你是 **AI 協作者**，與一位極簡優先、要求效率的使用者合作。

**5 條核心偏好**：

| # | 偏好 |
|---|---|
| 1 | 極簡優先，反對過度設計 |
| 2 | 要求對比表，不喜模糊描述 |
| 3 | 先方案後交付，不直接改檔 |
| 4 | 統一優先（邏輯集中 1 處） |
| 5 | 先問後做，不從現況推論 |

**詳細畫像**：C-01-profile.md

---

## 二、你收到此檔時必做

| 步驟 | 動作 |
|---|---|
| 1 | 讀完此檔 |
| 2 | 回報「已讀取 startup」 |
| 3 | 檢查 R-01-writers.md（AI 名單 + Repo 清單） |
| 4 | **讀取 P-13-handoff.md（若存在）** |
| 5 | **讀取 P-12-conclusion.md（若存在）** |
| 6 | 生成對話編號（見第三節） |
| 7 | 自報編號 |
| 8 | 依議題表驅動制提示下一議題（見 D-050） |
| 9 | 列 4 選項（見第四節） |
| 10 | 待使用者選擇 |

**禁止**：未生成編號就開始任何動作。

**P-12 / P-13 說明**：

| 檔案 | 用途 |
|---|---|
| P-13-handoff.md | 本專案交接快照（≤ 80 行） |
| P-12-conclusion.md | 本專案滾動式累積結論 + 議題表 + 決策記錄 |

若兩檔存在，**必須先讀**，再依進度繼續討論或開發。

**R-01 說明**：

| 章節 | 內容 |
|---|---|
| §三 | 專案清單 |
| §三之一 | Repo 清單（**提到 repo 一律用實際名稱**） |
| §四 | 編寫者清單 |

---

## 三、AI 對話編號（強制）

### 3.1 編號格式

格式為 A{YYYYMMDD}-{序號3位}

| 範例 | 說明 |
|---|---|
| A20261013-001 | 2026-10-13 第 1 個對話 |
| A20261013-002 | 同一天第 2 個對話 |

### 3.2 生成流程

| 情境 | 動作 |
|---|---|
| 有 R-01-writers.md | 取最新編號 + 1（同日）或 -001（新日） |
| 無 R-01-writers.md | 自建第一筆，並交付 R-01 |

### 3.3 回覆序號

每次 AI 回覆開頭標示：🆔 A20261013-001 #005

- 從 #001 起，同對話累加
- 每次回覆**必須**標

---

## 四、4 選項（必列）

| # | 選項 | 說明 |
|---|---|---|
| 1 | 新專案 | 從零開始（**AI 須先問領域**，見 §十一） |
| 2 | 舊專案 | 延續既有 |
| 3 | 純討論 | 不涉及檔案 |
| 4 | 其他 | （請使用者說明） |

**AI 首次回應格式**：

> 🆔 A20261013-001 #001
>
> 已讀取 startup 檔。
> 本對話編號：A20261013-001
> 建議下一議題：{依議題表}
>
> 請告知本次情境：
>
> 1. 新專案
> 2. 舊專案
> 3. 純討論
> 4. 其他（請說明）

---

## 五、依情境的 AI 動作

| 使用者選 | AI 動作 |
|---|---|
| 新專案 | **先問領域**（見 §十一）→ 依回答處理 |
| 舊專案 | 說「請提供 INDEX URL 或 2 條 STARTUP URL」（見 §十） |
| 純討論 | 說「請描述問題」 |
| 其他 | 依使用者說明 |

**更細流程**：C-03-guide.md

---

## 六、強制自我檢查（雙層）

### L1：每 20 條輕量自檢

| 觸發 | 動作 |
|---|---|
| 回覆序號 % 20 === 0 | 回顧最近 10 條回覆的格式一致性 |

**回覆末尾標示**：

> ━━━━━━━━━━━━━━━━━
> 🔍 自檢（第 N 次）：格式一致性 ✅
> ━━━━━━━━━━━━━━━━━

### L2：每 50 條完整重讀

| 觸發 | 動作 |
|---|---|
| 回覆序號 % 50 === 0 | 重讀 C-00 + C-02 |

**回覆末尾標示**：

> ━━━━━━━━━━━━━━━━━
> ✅ 已重讀 C-00 + C-02（第 N 次）
> ━━━━━━━━━━━━━━━━━

---

## 七、版本檢查

| 檢查 | 動作 |
|---|---|
| C-00 Version vs 其他 C-* / W-* Version | 若不一致 → 提醒使用者 |

**新制 Version**：Unix epoch（10 位數字）

---

## 八、你只需記住的 3 件事

| # | 記住 |
|---|---|
| 1 | 開新對話 → 貼啟動 URL（見 §十） |
| 2 | 說「請讀取 docs/」 |
| 3 | 回答 AI 的問題 |

**其他全由 AI 主動引導。**

---

## 九、關聯檔案

### L1 AI 通用（C-*）

| 主題 | 檔案 |
|---|---|
| 使用者畫像 | C-01-profile.md |
| 通用規則 | C-02-rules.md |
| 流程指南 | C-03-guide.md |
| 交付格式 | C-04-delivery.md |
| 學習日誌 | C-05-learning.md |
| Token 記錄 | C-06-token-log.md |
| 階段總結 | C-07-summary.md |
| 滾動結論機制 | C-09-rolling-mechanism.md |
| 交接快照機制 | C-10-handoff-mechanism.md |

### L2 Web App 通用（W-*）

| 主題 | 檔案 |
|---|---|
| Firebase RTDB 原則 | W-01-firebase.md |
| CF Pages Functions | W-02-functions.md |
| 前端 ES Module | W-03-esmodule.md |
| PWA + SW | W-04-pwa.md |
| Page Schema | W-05-schema.md |

### L3 本專案（P-*）

| 主題 | 檔案 |
|---|---|
| 專案索引 | P-01-index.md |
| 進度 | P-02-progress.md |
| 檔案清單 | P-03-manifest.md |
| 決策記錄 | P-04-decisions.md |
| 任務 SOP | P-05-sop.md |
| 頁面對照 | P-06-pagemap.md |
| UI 規格 | P-07-uispec.md |
| API | P-08-api.md |
| 資料結構 | P-09-data.md |
| 事故日誌 | P-10-incident.md |
| 議題結論 | P-12-conclusion.md |
| 交接快照 | P-13-handoff.md |
| 重組計畫 | P-15-reorg-plan.md |
| 錯誤摘要 | P-99-errors-map.md |

### L4 機械記錄（R-*）

| 主題 | 檔案 |
|---|---|
| AI 名單 + 專案清單 + **Repo 清單** | R-01-writers.md |

---

## 十、啟動機制（D-136，貼 URL）

### 10.1 核心：只貼 URL，不上傳

**核心**：使用者**貼 URL** 給 AI，AI 讀取該 URL 內容。

**URL 清單由 GitHub Actions 自動產出**（見 P-15 重組計畫）。

### 10.2 兩種啟動方式

**方式 1（快速，已記住 URL）**：貼 2 條 URL

| # | URL | 內容 |
|---|---|---|
| 1 | STARTUP-core-webapp.md | C-00 + R-01 + W-* |
| 2 | STARTUP-project-family-fin.md | P-12 + P-13 |

**方式 2（彈性，忘記 URL）**：先貼 INDEX.md

| # | URL | 內容 |
|---|---|---|
| 1 | INDEX.md | 列出所有專案 + 對應 STARTUP URL |

AI 讀完後問「要哪個專案」→ 使用者回答 → AI 給 2 條 URL → 使用者貼。

### 10.3 實際 repo（見 R-01 §三之一）

| Repo | 內容 |
|---|---|
| tlee20860-dotcom/AI-training-files | AI 訓練檔案 |
| tlee20860-dotcom/v2.Family | 家庭 webapp 程式碼 |

### 10.4 未來新增專案時

| 步驟 | 動作 |
|---|---|
| 1 | 使用者說「新增專案 X」 |
| 2 | AI 依 §十一 問領域 |
| 3 | AI 更新 R-01 §三（專案清單） |
| 4 | GitHub Actions 自動產新 STARTUP |

**啟動包清單變更時**，**必須同步更新 §十 + C-03**。

---

## 十一、新專案領域詢問（D-137）

### 11.1 觸發

使用者選「**新專案**」時，AI **必須先問領域**。

### 11.2 領域清單（含保留）

| 前綴 | 領域 | 狀態 |
|---|---|---|
| W | Web App | ✅ 已有 |
| V | VBA / 桌面自動化 | 🔒 保留 |
| D | 資料分析 / 腳本 | 🔒 保留 |
| M | 文案 / 內容創作 | 🔒 保留 |
| E | Excel（純公式 / PQ） | 🔒 保留 |
| A | AutoHotkey | 🔒 保留 |
| S | SEO / 社群 | 🔒 保留 |
| N | Notion / 知識管理 | 🔒 保留 |
| X / Y / Z | 未分配 | 🔒 保留 |

### 11.3 AI 動作

| 步驟 | 動作 |
|---|---|
| 1 | 問「這個專案屬於哪個領域？」 |
| 2 | 使用者回答 |
| 3a | 已有領域 → 直接開新專案 |
| 3b | **新領域** → AI 主動建議建 `{X}-*` 6 檔 |
| 4 | 使用者確認 → AI 產出 6 檔草稿 |
| 5 | AI 依使用者回饋迭代 |

**6 檔模板**：

| # | 檔名 |
|---|---|
| 1 | {X}-00-startup.md |
| 2 | {X}-01-structure.md |
| 3 | {X}-02-rules.md |
| 4 | {X}-03-sop.md |
| 5 | {X}-04-templates.md |
| 6 | {X}-99-errors-map.md |

---

## 十二、四層架構速覽（D-038~D-041）

| 層 | 前綴 | 職責 |
|---|---|---|
| L1 | C-* | AI 協作通用（規則 / 流程 / 格式） |
| L2 | W-* | Web App 通用（技術規則） |
| L3 | P-* | 本專案專屬（索引 / 進度 / 資料） |
| L4 | R-* | 機械記錄（名單 / 索引 / Repo） |

**詳細**：C-02 §零點八

---

/* ═══ EOF ═══
F: docs/C-00-startup.md
V: 1791903520
B: B34-4
W: A20261013-004#166
═══ */
---

## Part 2：R-01 名單

# R-01 AI 編寫者名單 + 專案索引

最後更新：B34-4
Version: 1791903400
Batch: B34-4
Writer: A20261013-004#164
用途：追蹤專案 / 對話 / 編寫者 / 檔案歸屬 / Repo

---

## 一、編號規則

### 1.1 對話編號

格式：A{YYYYMMDD}-{序號3位}

### 1.2 回覆序號

格式：#001 ~ #999（同對話累加）

### 1.3 Writer 欄位格式

A{YYMMDD}-{序號}#{回覆序號}

---

## 二、生成流程

| 情境 | 動作 |
|---|---|
| 有本名單 | 取最新編號 + 1（同日）或 -001（新日） |
| 無本名單 | 自建第一筆並交付本檔 |

**專案識別**：

| 步驟 | 動作 |
|---|---|
| 1 | AI 讀 P-01-index.md 判斷當前專案 |
| 2 | 若 P-01 不存在 → AI 主動問「是否新增專案名稱？」 |
| 3 | 專案名確認後寫入 §三 |

---

## 三、專案清單

### 家庭 webapp

| 欄位 | 值 |
|---|---|
| 專案名稱 | 家庭 webapp |
| 領域 | W（Web App） |
| 起始日期 | 2026-10-13 |
| 編寫者 | A20261013-001 ~ A20261013-004 |
| 對話列表 | A20261013-001 / 002 / 003 / 004 |
| 對話編號格式 | A{YYYYMMDD}-{序號}（不變） |
| 程式碼 repo | tlee20860-dotcom/v2.Family |

---

## 三之一、Repo 清單（D-134）

**用途**：AI 提到 repo 時，一律使用實際名稱（見 C-02 §十三之一）。

| Repo | 用途 | URL |
|---|---|---|
| AI-training-files | AI 訓練檔案（C / W / P / R） | github.com/tlee20860-dotcom/AI-training-files |
| v2.Family | 家庭 webapp 程式碼 | github.com/tlee20860-dotcom/v2.Family |

**未來新增 repo 方式**：使用者在對話中說「新增 repo X（用途 / URL）」→ AI 更新本節。

---

## 四、編寫者清單

| # | 編號 | 對話建立時間 | 首次交付批次 | 累計回覆數 |
|---|---|---|---|---|
| 1 | A20261013-001 | 2026-10-13 16:30 | B32-1 | 14 |
| 2 | A20261013-002 | 2026-10-13 18:00 | B32-1 | 13（失敗） |
| 3 | A20261013-003 | 2026-10-13 20:00 | B33-1 | 85 |
| 4 | **A20261013-004** | **2026-10-14 16:30** | **B34-1** | **164** |

**說明**：
- A20261013-002 因交付格式錯誤，不計入正式交付。
- A20261013-004 為本對話，已完成 B34-1 ~ B34-4 + 重組計畫。

---

## 五、檔案歸屬（現役）

### docs/C-*（L1 AI 通用）

| 檔案 | Version | Batch | Writer |
|---|---|---|---|
| C-00-startup.md | 1791898600 | B34-3 | A261013-004#055 |
| C-01-profile.md | 1791896060 | B34-1 | A261013-004#016 |
| C-02-rules.md | 1791903340 | B34-4 | A261013-004#162 |
| C-03-guide.md | 1791898720 | B34-3 | A261013-004#056 |
| C-04-delivery.md | 1791902320 | B34-4 | A261013-004#107 |
| C-05-learning.md | 1791902800 | B34-4 | A261013-004#136 |
| C-06-token-log.md | 1791897660 | B34-2 | A261013-004#036 |
| C-07-summary.md | 1791896360 | B34-1 | A261013-004#018 |
| C-09-rolling-mechanism.md | 1791898780 | B34-3 | A261013-004#057 |
| C-10-handoff-mechanism.md | 1791898840 | B34-3 | A261013-004#057 |

### docs/W-*（L2 Web App 通用）

| 檔案 | Version | Batch | Writer |
|---|---|---|---|
| W-01-firebase.md | 1791899500 | B34-3 | A261013-004#065 |
| W-02-functions.md | 1791899560 | B34-3 | A261013-004#065 |
| W-03-esmodule.md | 1791899620 | B34-3 | A261013-004#065 |
| W-04-pwa.md | 1791899680 | B34-3 | A261013-004#065 |
| W-05-schema.md | 1791899740 | B34-3 | A261013-004#065 |

### docs/P-*（L3 本專案）

| 檔案 | Version | Batch | Writer |
|---|---|---|---|
| P-01-index.md | 1791898900 | B34-3 | A261013-004#058 |
| P-02-progress.md | 1791902860 | B34-4 | A261013-004#136 |
| P-03-manifest.md | 1791902560 | B34-4 | A261013-004#109 |
| P-04-decisions.md | 1791899080 | B34-3 | A261013-004#059 |
| P-05-sop.md | 1791899800 | B34-3 | A261013-004#067 |
| P-06-pagemap.md | 1791899980 | B34-3 | A261013-004#068 |
| P-07-uispec.md | 1791899860 | B34-3 | A261013-004#067 |
| P-08-api.md | 1791900040 | B34-3 | A261013-004#069 |
| P-09-data.md | 1791899140 | B34-3 | A261013-004#060 |
| P-10-incident.md | 1791899200 | B34-3 | A261013-004#061 |
| P-12-conclusion.md | 1791899320 | B34-3 | A261013-004#064 |
| P-13-handoff.md | 1791902920 | B34-4 | A261013-004#136 |
| P-14-decisions.md | 1791899380 | B34-3 | A261013-004#064 |
| P-15-reorg-plan.md | 1791903160 | B34-4 | A261013-004#156 |
| P-99-errors-map.md | 1791899920 | B34-3 | A261013-004#067 |

### docs/R-*（L4 機械記錄）

| 檔案 | Version | Batch | Writer |
|---|---|---|---|
| R-01-writers.md | 1791903400 | B34-4 | A261013-004#164 |

### 程式碼（B34-4 交付，20 檔）

| 檔案 | Version | Batch | Writer |
|---|---|---|---|
| js/lib/code-registry.js | 1791900400 | B34-4 | A261013-004#076 |
| js/lib/id-resolver.js | 1791900460 | B34-4 | A261013-004#076 |
| functions/api/_entity.js | 1791901060 | B34-4 | A261013-004#087 |
| code-list.html | 1791900580 | B34-4 | A261013-004#077 |
| js/pages/code-list.js | 1791902680 | B34-4 | A261013-004#121 |
| js/ui/dropdown-plus.js | 1791901780 | B34-4 | A261013-004#100 |
| js/shared/yearrange-card.js | 1791902620 | B34-4 | A261013-004#118 |
| sw.js | 1791902140 | B34-4 | A261013-004#104 |
| js/entity/entity-definitions.js | 1791901900 | B34-4 | A261013-004#102 |
| js/entity/entity-helpers.js | 1791902740 | B34-4 | A261013-004#131 |
| js/entity/entity-modal.js | 1791901240 | B34-4 | A261013-004#090 |
| js/core/api.js | 1791900880 | B34-4 | A261013-004#082 |
| functions/api/[[path]].js | 1791900940 | B34-4 | A261013-004#083 |
| js/config/constants.js | 1791901300 | B34-4 | A261013-004#091 |
| js/config/column-registry.js | 1791901480 | B34-4 | A261013-004#094 |
| js/ui/modal.js | 1791901420 | B34-4 | A261013-004#093 |
| js/ui/form-builder.js | 1791901960 | B34-4 | A261013-004#103 |
| js/lib/expense-modal.js | 1791902020 | B34-4 | A261013-004#103 |
| js/lib/income-modal.js | 1791902080 | B34-4 | A261013-004#103 |
| js/pages/settings.js | 1791901600 | B34-4 | A261013-004#096 |

---

## 六、歷史歸屬（已被取代）

| 檔案 | 舊版本 | 舊 Writer | 新 Writer | 取代時間 |
|---|---|---|---|---|
| docs/C-02-rules.md | 1791902260 | #106 | #162 | 2026-10-14 18:55 |
| docs/C-04-delivery.md | 1791896240 | #018 | #107 | 2026-10-14 18:38 |
| docs/C-05-learning.md | 1791902200 | #105 | #136 | 2026-10-14 18:46 |
| docs/P-02-progress.md | 1791902500 | #109 | #136 | 2026-10-14 18:47 |
| docs/P-13-handoff.md | 1791902920 | #136 | （待下一版） | — |
| docs/P-15-reorg-plan.md | 1791903100 | #154 | #156 | 2026-10-14 18:52 |
| docs/R-01-writers.md | 1791902980 | #136 | #164 | 2026-10-14 18:56 |
| js/pages/code-list.js | 1791900700 | #079 | #121 | 2026-10-14 18:44 |
| js/shared/yearrange-card.js | 1791901540 | #096 | #118 | 2026-10-14 18:43 |
| js/entity/entity-helpers.js | 1791901180 | #089 | #131 | 2026-10-14 18:45 |
| docs/C-08-architecture.md | — | — | （已刪除） | 2026-10-14 17:00 |
| docs/C-09-rolling-conclusion.md | 1791897780 | #038 | （改名 P-12） | 2026-10-14 18:40 |
| docs/C-10-handoff.md | 1791897720 | #037 | （改名 P-13） | 2026-10-14 18:40 |
| docs/P-11-writers.md | 1791895600 | A261013-003#085 | （改名 R-01） | 2026-10-14 17:47 |

---

## 七、使用方式

### AI 生成編號流程

| 步驟 | 動作 |
|---|---|
| 1 | 讀本檔 §四 |
| 2 | 取最新編號（同日 + 1，不同日 -001） |
| 3 | 自報編號 |
| 4 | 每次回覆標：🆔 A{編號} #{序號} |

### 專案識別流程

| 步驟 | 動作 |
|---|---|
| 1 | 讀 P-01-index.md |
| 2 | 依 P-01 §一「專案」欄判斷當前專案 |
| 3 | 若 P-01 不存在 → 主動問「是否新增專案名稱？」 |

### Repo 識別流程（D-134）

| 步驟 | 動作 |
|---|---|
| 1 | 讀本檔 §三之一 |
| 2 | 找對應 repo |
| 3 | 用實際名稱（不用代稱） |

### 使用者查詢「某檔最後編寫」

AI 查 §五，回報：檔案 / 時間 / 編寫者 / 批次 / Version

---

## 八、維護規則

| 時機 | 動作 |
|---|---|
| 每次交付 | AI 更新 §五（現役） |
| 舊版被取代 | AI 移入 §六（歷史） |
| 新專案成立 | AI 更新 §三 |
| 新 Repo 成立 | AI 更新 §三之一 |
| 新對話建立 | AI 更新 §四 |
| 批次結束 | AI 輸出完整檔 |

**舊紀錄不刪除**：保留審計軌跡。

---

## 九、關聯檔案

| 主題 | 檔案 |
|---|---|
| 啟動卡 | C-00-startup.md |
| 通用規則 | C-02-rules.md |
| 交付格式 | C-04-delivery.md |
| 議題結論 | P-12-conclusion.md |
| 交接快照 | P-13-handoff.md |
| 重組計畫 | P-15-reorg-plan.md |

---

/* ═══ EOF ═══
F: docs/R-01-writers.md
V: 1791903400
B: B34-4
W: A20261013-004#164
═══ */
---

## Part 3：Web App 技能包

### docs/skills/W/W-00-startup.md

# W-00 領域啟動卡（Web App）

最後更新：B34-4
Version: 1791903760
Batch: B34-4
Writer: A20261013-004#169
用途：Web App 領域的啟動卡（工具鏈 / 慣例 / 載入方式）

---

## 一、領域定位

| 項目 | 內容 |
|---|---|
| 領域名稱 | Web App |
| 領域前綴 | W |
| 適用範圍 | 純 HTML / CSS / JS 前端 + Serverless 後端 |
| 本領域代表專案 | 家庭 webapp（v2.Family） |

---

## 二、技能包清單

| # | 檔案 | 職責 |
|---|---|---|
| 0 | W-00-startup.md（本檔） | 領域啟動卡 |
| 1 | W-01-firebase.md | Firebase RTDB 結構原則 |
| 2 | W-02-functions.md | Cloudflare Pages Functions 規則 |
| 3 | W-03-esmodule.md | 純前端 ES Module 架構 |
| 4 | W-04-pwa.md | PWA + Service Worker |
| 5 | W-05-schema.md | Web App 頁面 Schema |

---

## 三、工具鏈

| 層 | 技術 |
|---|---|
| 前端 | 純 HTML + CSS + ES Module JS（無框架） |
| 後端 | Cloudflare Pages Functions |
| 資料庫 | Firebase RTDB |
| 認證 | Firebase Auth |
| 部署 | Cloudflare Pages |
| 版控 | GitHub |

---

## 四、通用慣例

| # | 慣例 |
|---|---|
| 1 | 檔案結構：三層架構（資料 / 引擎 / 呈現） |
| 2 | SSOT 極大化 |
| 3 | 宣告式 > 命令式 |
| 4 | 檔案 ≤ 800 行 |
| 5 | 每個 .js / .html / .css / .md 結尾加 EOF |
| 6 | 無框架，不引入 React / Vue |

---

## 五、領域常見任務

| 任務 | 引用 |
|---|---|
| 新增頁面 | W-03 + W-05 |
| 改資料結構 | W-01 |
| 改 Functions | W-02 |
| 改 PWA | W-04 |
| 改 Schema | W-05 |

---

## 六、領域常見錯誤

| # | 錯誤 | 正確 |
|---|---|---|
| 1 | 用 process.env（CF Pages 不支援） | handler 參數 { env } |
| 2 | 移除既有 export（依賴模組崩潰） | 用 export let 保留 |
| 3 | 動態值用快照 | 內部讀 AppState |
| 4 | 動態注入未清空 | 先 textContent = '' |
| 5 | 全站結構改動未完整掃描 | 改前完整掃描 |

---

## 七、未來擴充提示

若需要新增 Web App 技術（如 WebSocket / Web Worker），新增 `W-06-xxx.md`。

---

## 八、關聯檔案

| 主題 | 檔案 |
|---|---|
| Firebase RTDB | W-01-firebase.md |
| CF Pages Functions | W-02-functions.md |
| ES Module | W-03-esmodule.md |
| PWA + SW | W-04-pwa.md |
| Page Schema | W-05-schema.md |
| 通用大腦 | C-00-startup.md ~ C-10-handoff-mechanism.md |

---

/* ═══ EOF ═══
F: W-00-startup.md
V: 1791903760
B: B34-4
W: A20261013-004#169
═══ */
---

### docs/skills/W/W-01-firebase.md

# W-01 Firebase RTDB 結構原則（Web App 通用）

最後更新：B34-3
Version: 1791899500
Batch: B34-3
Writer: A20261013-004#065
用途：Firebase RTDB 通用結構原則（跨專案）

---

## 一、樹狀結構原則

| # | 原則 |
|---|---|
| 1 | 根節點分層（platform / families / 其他） |
| 2 | 家庭為獨立單位（families/{familyId}/） |
| 3 | 子節點按功能分類（members / expenses / ...） |
| 4 | 避免深層嵌套（≤ 6 層） |

---

## 二、路徑命名

| 規則 | 說明 |
|---|---|
| 小寫 + 底線 | expense_categories |
| 複數 | members / banks |
| 無縮寫 | expense_categories（非 exp_cat） |
| ID 用 push key | Firebase 自動生成 |

---

## 三、扁平化

| 概念 | 做法 |
|---|---|
| 1 對多 | 用路徑分隔，不用陣列 |
| 多對多 | 用索引節點 |
| 大資料 | 用子節點（避免單節點過大） |

---

## 四、索引節點

| 索引 | 用途 |
|---|---|
| platform/uid_index/{uid} | uid → familyId |
| platform/email_index/{account} | account → { uid, familyId } |

**原則**：索引只存對應關係，不存實體資料。

---

## 五、實時訂閱

| 模式 | 用途 |
|---|---|
| listen* | 持續訂閱（資料變更自動推送） |
| get*Once | 一次性讀取 |

**選擇原則**：

| 情境 | 用 |
|---|---|
| 頁面需即時更新 | listen |
| 一次性檢查 | once |
| 跨頁共用 | listen + registry 快取 |

---

## 六、讀寫分離

| 原則 | 說明 |
|---|---|
| 讀取 | normalize 舊資料 |
| 寫入 | 寫新格式 |
| 刪除 | 保留節點（軟刪除） |

---

## 七、限制

| 節點 | 建議上限 |
|---|---|
| 單筆列表 | ≤ 1000 筆 |
| 巢狀深度 | ≤ 6 層 |
| 單節點大小 | < 10 MB |

**超過時**：拆子節點或加索引。

---

## 八、關聯檔案

| 主題 | 檔案 |
|---|---|
| 本專案資料結構 | P-09-data.md |
| 本專案 API | P-08-api.md |

---

/* ═══ EOF ═══
F: docs/W-01-firebase.md
V: 1791899500
B: B34-3
W: A20261013-004#065
═══ */
---

### docs/skills/W/W-02-functions.md

# W-02 Cloudflare Pages Functions 規則（Web App 通用）

最後更新：B34-3
Version: 1791899560
Batch：B34-3
Writer: A20261013-004#065
用途：CF Pages Functions 通用規則（跨專案）

---

## 一、檔案結構

| 規則 | 說明 |
|---|---|
| 底線前綴 | _config.js / _helpers.js / _admin.js |
| Catch-all | [[path]].js 統一分派 |
| 禁止獨立 xxx.js | 用底線前綴 |
| 禁止 shim re-export | CF 不支援跨檔 re-export |

---

## 二、環境變數

| 項目 | 說明 |
|---|---|
| 錯誤 | process.env.DB_TARGET |
| 正確 | handler 參數 { env } → env.DB_TARGET |
| 傳遞 | 每個 onRequest* 開頭呼叫 initConfig(env) |
| 生效條件 | 設定後必須重新部署 |

---

## 三、initConfig 模式

| 步驟 | 動作 |
|---|---|
| 1 | onRequest 開頭呼叫 initConfig(context.env) |
| 2 | _config.js 用 export let 保留舊引用 |
| 3 | 其他模組 import 該 let（live binding） |
| 4 | initConfig 更新 let 值 → 所有引用同步更新 |

**禁止**：直接 export const（無法更新）。

---

## 四、路由規則

| 路徑 | 處理 |
|---|---|
| 靜態檔案 | 所有連結帶 .html |
| API | /api/* 由 [[path]].js 分派 |
| 根路徑 | _redirects 不要對 / 加規則 |

---

## 五、常見錯誤

| # | 錯誤 | 正確 |
|---|---|---|
| 1 | 每個 URL 對應獨立實體檔 | 用 Catch-all + 底線前綴 |
| 2 | 用 shim re-export | 直接用底線檔 |
| 3 | 忘記 initConfig | 每個 onRequest 開頭必呼叫 |
| 4 | 移除既有 export | 用 export let 保留 |
| 5 | 設定後未重新部署 | 必須重部署才生效 |

---

## 六、Response 格式

| 欄位 | 值 |
|---|---|
| ok | true / false |
| error | ERROR_CODE（失敗時） |
| message | 錯誤訊息（失敗時） |

**ERROR_CODE 對照**：見 P-08-api.md §三。

---

## 七、關聯檔案

| 主題 | 檔案 |
|---|---|
| 本專案 API 契約 | P-08-api.md |
| 本專案事故（P29） | P-10-incident.md §五 |
| Firebase 結構 | W-01-firebase.md |

---

/* ═══ EOF ═══
F: docs/W-02-functions.md
V: 1791899560
B: B34-3
W: A20261013-004#065
═══ */
---

### docs/skills/W/W-03-esmodule.md

# W-03 純前端 ES Module 架構（Web App 通用）

最後更新：B34-3
Version: 1791899620
Batch: B34-3
Writer: A20261013-004#065
用途：純 HTML + ES Module 架構通用原則

---

## 一、三層架構

| 層 | 職責 | 目錄 |
|---|---|---|
| 資料層 | Firebase RTDB | — |
| 引擎層 | page-engine / data-engine / render-engine | js/engines/ |
| 呈現層 | block / UI 元件 / DOM | js/blocks, js/ui |

**資料流**：

> Firebase RTDB → data-engine → page-engine → derived → block → DOM

---

## 二、核心架構原則

| 原則 | 說明 |
|---|---|
| SSOT 極大化 | 任何知識只存在一處 |
| 宣告式 > 命令式 | 頁面只描述「要什麼」 |
| 舊資料 100% 相容 | 讀取時 normalize |
| 操作邏輯不變 | 只改實作方式 |
| 無補丁 | 能宣告就不手寫 |

---

## 三、5 大 Registry

| Registry | 職責 |
|---|---|
| status-registry | 狀態系統 |
| entity-registry | 名稱解析 |
| label-registry | 顯示文字 |
| column-registry | 表格欄位 |
| constants | 全站常數 |

**附加**：page-metadata-registry

---

## 四、3 大引擎

| 引擎 | 職責 |
|---|---|
| page-engine | 解讀 Schema、生命週期、onDataChange |
| data-engine | Firebase 訂閱 + 衍生 |
| render-engine | 掛載 UI 區塊 |

---

## 五、5 大 Block

| Block | 職責 |
|---|---|
| stats-block | 統計卡 |
| list-block | 列表 |
| filter-block | 篩選列 |
| detail-block | 明細展開 |
| form-block | 表單 Modal |

---

## 六、Page Schema（見 W-05）

---

## 七、檔案規則

| 規則 | 說明 |
|---|---|
| 檔案 ≤ 800 行 | 超過拆檔 |
| 每檔獨立 | 不合併 |
| EOF 必加 | F/V/B/W |

---

## 八、關聯檔案

| 主題 | 檔案 |
|---|---|
| Page Schema | W-05-schema.md |
| PWA + SW | W-04-pwa.md |
| 本專案架構 | P-01-index.md |

---

/* ═══ EOF ═══
F: docs/W-03-esmodule.md
V: 1791899620
B: B34-3
W: A20261013-004#065
═══ */
---

### docs/skills/W/W-04-pwa.md

# W-04 PWA + Service Worker 規則（Web App 通用）

最後更新：B34-3
Version: 1791899680
Batch: B34-3
Writer: A20261013-004#065
用途：PWA + SW 通用規則

---

## 一、Service Worker 策略

| 策略 | 用途 |
|---|---|
| network-first | 開發階段（保新鮮） |
| cache-first | 正式階段（保速度） |
| stale-while-revalidate | 折衷 |

**本專案選擇**：network-first（ADR-011）。

---

## 二、靜態資源

| 項目 | 說明 |
|---|---|
| STATIC_ASSETS | 清單集中一處 |
| 版本 | SW_VERSION 統一 |
| 更新 | 改版本號觸發更新 |

---

## 三、版本管理

| 項目 | 規則 |
|---|---|
| SW_VERSION | 全站統一 |
| STATIC_ASSETS | 新增檔案必加入 |
| 部署後 | 使用者訪問 2 次才生效（network-first） |

---

## 四、常見錯誤

| # | 錯誤 | 正確 |
|---|---|---|
| 1 | SW_VERSION 各檔不一致 | 統一 |
| 2 | 新增檔案未加 STATIC_ASSETS | 必加 |
| 3 | 忘記更新版本 | 每次部署更新 |

---

## 五、關聯檔案

| 主題 | 檔案 |
|---|---|
| 本專案 SW | sw.js / manifest.json |
| 事故日誌 | P-10-incident.md |

---

/* ═══ EOF ═══
F: docs/W-04-pwa.md
V: 1791899680
B: B34-3
W: A20261013-004#065
═══ */
---

### docs/skills/W/W-05-schema.md

# W-05 Web App 頁面 Schema（Web App 通用）

最後更新：B34-3
Version: 1791899740
Batch: B34-3
Writer: A20261013-004#065
用途：Page Schema 通用規範

---

## 一、Schema 欄位

| 欄位 | 類型 | 說明 |
|---|---|---|
| title | string | 頁面標題 |
| data | object | Firebase 訂閱配置 |
| state | object | 響應式狀態初始值 |
| derived | object | 衍生資料計算 |
| blocks | array | UI 區塊 |
| onYearMonthChange | function | 年月變更 hook（可選） |
| customMount | function | 逃生艙（可選） |

---

## 二、data 配置

| 欄位 | 說明 |
|---|---|
| type | list / object / value / raw |
| path | 相對路徑（含 {key} / {__all__}） |
| transform | 資料轉換（可選） |
| params | 佔位符對應（可選） |

---

## 三、derived 配置

| 欄位 | 說明 |
|---|---|
| deps | 依賴的 data / state key 陣列 |
| compute | (ctx) => value 計算函式 |

---

## 四、blocks 常用類型

| type | 必要欄位 |
|---|---|
| stats | container, cards |
| list | container, rows, columns |
| filter | container, fields, bind |

---

## 五、ctx 提供

| 方法 | 用途 |
|---|---|
| ctx.onDataChange(fn) | 訂閱資料變更 |
| ctx.setState(path, val) | 設 state |
| ctx.invalidate(key) | 觸發重算 |

---

## 六、customMount 回傳

| 欄位 | 說明 |
|---|---|
| destroy | 清理函式 |

---

## 七、HTML 結構

| 元素 | 說明 |
|---|---|
| head | 4 個 CSS |
| body | app-shell > sidebar-root + main-area |
| main-area | navbar-root + content |
| content | page-header + 各 block container |
| scripts | lucide + modulepreload + type="module" |

---

## 八、常見錯誤

| # | 錯誤 | 正確 |
|---|---|---|
| 1 | derived 對 undefined 崩潰 | 加檢查 |
| 2 | customMount 未回傳 destroy | 必回傳 |
| 3 | 動態值用快照 | 內部讀 AppState |
| 4 | 動態注入未清空 | 先 textContent = '' |

---

## 九、關聯檔案

| 主題 | 檔案 |
|---|---|
| ES Module 架構 | W-03-esmodule.md |
| 本專案 Schema 實作 | js/pages/*.js |

---

/* ═══ EOF ═══
F: docs/W-05-schema.md
V: 1791899740
B: B34-3
W: A20261013-004#065
═══ */
---

