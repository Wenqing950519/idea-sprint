# Idea Sprint｜自主思考引導

讓 AI 引導你思考，而不是替你交出漂亮但空泛的創意。

適合研究、競賽、商業與創作的早期探索。每個人各自使用：從自己的觀察或閱讀疑問起步，預設最多六次回答、每次一個核心問題，最後得到一張可追溯的推導卡。已有材料就跳過，不必跑完固定問卷；隨時說「先整理」即可結束。

## 開始使用

使用支援 Agent Skills 的工具時，將本專案的 `SKILL.md`、`agents/`、`references/` 放入同一個 `idea-sprint` skill 資料夾，再依工具的個人 skill 安裝流程啟用。可用以下指令開始：

> 請用 idea-sprint 引導我探索方向，最多六輪、每次一問；不要替我產生創意，最後整理推導卡。

若使用的聊天工具沒有 skill 安裝功能，可提供 `SKILL.md` 與 `references/checkpoint.md` 的內容，明確要求依這套規則執行。單純貼 GitHub 連結不保證 AI 已讀到內容；先請它確認讀到了規則。

## 它會與不會做什麼

| 會做 | 不會做 |
| --- | --- |
| 從你的經驗、案例、閱讀或好奇開始 | 替你列十個題目、推薦市場或產品 |
| 改成具體、白話且可回答的問題 | 連續追問抽象問題，直到你疲倦 |
| 解釋概念與提供有來源的資料 | 把搜尋結果當成你自己的判斷 |
| 分清觀察、假設、外部證據、AI 方法 | 把「對、都可以」加工成完整論證 |
| 在上限前後留下成果與缺口 | 為了填表而延長，或把缺口藏起來 |

## 如何收斂

預設最多六次回答；要求簡短可用四次；已有內容可提前完成。連續兩次沒有材料時，整理目前缺口並給一個最小觀察任務。AI 解釋概念與查資料不增加題號，也不應重置已消耗的回答額度。

最後交付：我的觀察 → 我想追的問題與理由 → 我的解釋／假設 → 支持、反對與缺口 → 下一步。未形成方向或尚無證據都可以如實交付；本輪結束不代表想法已被驗證。

只有使用者要求再深入，才圍繞一個缺口另開單元。A–E（Discover、Define、Diverge、Validate、Decide）是 AI 內部路由，不是使用者必須通過的五關。

## 為什麼限制 AI 代想

這個版本用於需要保留思考自主性的個人探索。不因「直接幫我想」自動切換共同發想模式；使用者可明確退出此流程。這是對話規則，不是無法繞過的技術鎖，也不能證明使用者的想法沒有其他 AI 參與。

六輪與四輪是待持續試用的操作預設，不是研究驗證的最優數值。目標是讓過程可預期，同時避免為了速度把假設當結論。

## 設計參考

以下方法用於啟發階段交付、查證與結束條件，不代表本 skill 已有實證效果；本版不包含團隊協作或投票功能。

- [thoughtbot/design-sprint](https://github.com/thoughtbot/design-sprint)：理解、發散、收斂、測試；專案已封存，作為歷史流程參考。
- [product-on-purpose/pm-skills — Design Sprint](https://github.com/product-on-purpose/pm-skills/blob/main/_workflows/design-sprint.md)：以明確輸入輸出串接階段。
- [GitLab — Design and run workshops](https://handbook.gitlab.com/handbook/upstream-studios/experience-research/design-run-workshops/)：階段要有產出，保留未處理議題，避免無限討論。
- [Strategyzer — Test Card](https://www.strategyzer.com/library/validate-your-ideas-with-the-test-card)：將假設、測試、指標與門檻分開。

## 驗收

見 [行為情境](evals/scenarios.md) 與 [本版試跑紀錄](evals/results.md)。情境試跑只能觀察有限案例，不代表在所有模型與長對話都能遵守。

核心技能檔為 [SKILL.md](SKILL.md)，推導卡規則為 [references/checkpoint.md](references/checkpoint.md)。本專案不收錄使用者的真實訪談或私人研究資料。
