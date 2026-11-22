姜不應 RAG 聊天程式

檔案：
- index.html：聊天介面與本地檢索/回覆邏輯
- knowledge.json：姜不應讀取的角色與世界知識庫

使用方式：
1. 將 index.html 與 knowledge.json 放在同一個資料夾。
2. 用 VS Code 開啟該資料夾。
3. 使用 Live Server 開啟 index.html。
4. 不要直接用 file:// 雙擊開啟，因為瀏覽器可能阻擋 fetch 讀取 JSON。

限制：
- 不使用 AI API、不連接生成式 AI。
- 這是本地 JSON 知識庫＋關鍵字檢索＋規則式回覆，不是向量檢索或 LLM 型完整 RAG。
- knowledge.json 可直接編輯擴充。請保留 certainty 欄位，避免把傳聞寫成確定事實。
