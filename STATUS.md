# STATUS

階段：**已上線使用**（https://nccu-huaxia.github.io/HuaXia/），2026-10 完成介面改版。

- 網站：GitHub Pages（repo `nccu-huaxia/HuaXia`，2026-11 從舊帳號搬過來），推上 `main` 約 1–3 分鐘生效
- 資料庫：Supabase（2026-11 Eddy 說已轉到「政大華夏國樂社」組織）；改資料庫要先在 SQL Editor 執行 `supabase/schema.sql`，再合併網站的修改
- Supabase 的 Site URL／Redirect URLs、Secret `SITE_URL` 已改成新網址（2026-11-10）
- 換網址公告已發（2026-11-10）
- 「用 Discord 登入」改用社團自己的 Discord 應用程式「華夏恐ㄎ一ㄤ龍」（2026-11-10）；DC 機器人（每晚提醒、✅／請假按鈕）本來就是同一個應用程式
- 示範模式（`?demo`）已移除
- 每晚提醒的 Edge Function 實際名稱是 `daily-reminder-`（多一個 `-`），排程（`supabase/cron.sql`）呼叫這個名字

## 待辦：開工時先提醒使用者（swiming）
1. **Google 行事曆同步要不要刪**（2026-11-14 使用者說有空再想，要提醒）：先請他看網站「我的」頁面「加到我的行事曆」那一區。寫「行事曆還沒建立好」= 沒用過，可以直接刪（拿掉我的頁行事曆區與 Google 信箱欄、設定頁 Google 行事曆區、events.js／members.js 呼叫 calendar-sync；不用改資料庫）。有加入按鈕 = 有人在用，刪之前要發公告請大家移除手機上的華夏行事曆；不刪的話要請 Eddy 把 Google Cloud 專案擁有者加給社團帳號。
2. Eddy 交接：GitHub 組織確認有其他 Owner 後移除 oshigirimoquan-coder；Supabase 組織 Team 確認使用者是 Owner 後移除 Eddy。
3. 還沒回報：從 Discord 點進網站是否還要每次重新登入；指導老師登入後「出席率總表」是否看得到全團。

最新紀錄見 `HANDOFF.md`；待決事項見 `docs/open-questions.md`。
