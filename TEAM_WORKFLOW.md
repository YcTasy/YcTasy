# AI 團隊 + LM Studio 協作 GUI-style Checklist

此清單設計給使用 **GitHub + LM Studio + Notion + Slack** 的 AI 團隊，確保多人協作時能保持一致性、透明度與高效率。

---

## 🛠️ 環境準備
- [ ] **GitHub/GitLab**：建立專案倉庫，包含提示詞 (System Prompt)、Persona JSON、回測程式碼。
- [ ] **LM Studio**：安裝並設定本地推理環境，確保每位成員能載入相同模型。
- [ ] **Notion**：建立知識庫，存放策略設計、回測報告、最佳化紀錄。
- [ ] **Slack**：建立團隊頻道，整合 GitHub 與 LM Studio API 通知。

---

## 📂 GitHub 協作流程
- [ ] 建立 **主分支 (main)**：存放穩定版本的提示詞與程式碼。
- [ ] 建立 **開發分支 (dev)**：團隊成員在此提交新策略或人設更新。
- [ ] 使用 **Pull Request**：確保程式碼與提示詞更新經過審核。
- [ ] 設定 **CI/CD**：自動測試回測程式碼，確保策略正確性。

---

## 🖥️ LM Studio 使用規範
- [ ] 每位成員安裝相同版本的 LM Studio。
- [ ] 使用統一的 **System Prompt** 與 **Persona JSON**。
- [ ] 啟動時指定 LAN API，確保團隊能共享測試結果。
- [ ] 在回測時輸出結果到 GitHub 或 W&B。

---

## 📖 Notion 知識庫
- [ ] 建立 **策略設計頁面**：描述策略邏輯與使用情境。
- [ ] 建立 **回測報告頁面**：存放回測數據、圖表與結論。
- [ ] 建立 **最佳化紀錄頁面**：追蹤不同模型版本與調整。
- [ ] 建立 **人設管理頁面**：存放 Persona JSON 與提示詞。

---

## 💬 Slack 整合
- [ ] 建立 **#lmstudio-notify** 頻道：接收模型載入與回測完成通知。
- [ ] 整合 **GitHub**：當有 Pull Request 或 Commit 時自動通知。
- [ ] 整合 **LM Studio API**：回測完成後自動推送結果到 Slack。
- [ ] 設定 **提醒與排程**：定期檢查模型更新與策略迭代。

---

## 🎯 團隊工作流範例
1. 成員在 **GitHub dev 分支** 提交新策略程式碼與提示詞。
2. CI/CD 自動執行回測，結果上傳到 **GitHub Actions/W&B**。
3. **Slack** 自動通知團隊回測完成。
4. 團隊在 **Notion** 撰寫回測報告與最佳化紀錄。
5. 經過審核後合併到 **main 分支**，並更新 LM Studio Persona。

---

✅ 這份 Checklist 能幫助 AI 團隊在 LM Studio 上保持一致的協作流程，避免人設不同步或模型版本不一致的問題。
