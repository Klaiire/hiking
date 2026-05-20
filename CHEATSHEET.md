# 嚮導考試檔案同步指令說明

## 快速同步（Terminal 指令）

```bash
sync-exam
```

**做了什麼：**
1. 把 `/Documents/Claude Project/嚮導考試/` 裡所有 `.html` 複習檔案複製到本機 repo
2. 自動 `git commit`（存檔紀錄）
3. 自動 `git push`（推上 GitHub）

> 第一次使用前，需先執行一次 `source ~/.zshrc` 讓指令生效。之後開新 Terminal 視窗就不用了。

---

## 告訴 Claude 同步（對話指令）

直接跟 Claude 說：

> 「幫我同步考試檔案」

Claude 會自動執行複製＋commit＋push，不需要你打任何 Terminal 指令。

---

## 相關路徑備忘

| 說明 | 路徑 |
|------|------|
| HTML 來源（Claude 產出） | `/Users/claireston/Documents/Claude Project/嚮導考試/` |
| 本機 Git repo | `~/Documents/Github/hiking/嚮導考試/` |
| GitHub 網址 | https://github.com/Klaiire/hiking |

---

## 其他常用 git 指令

```bash
# 查看目前狀態（有沒有未推的變更）
cd ~/Documents/Github/hiking && git status

# 手動推上去（自訂 commit 訊息）
cd ~/Documents/Github/hiking && git add 嚮導考試/ && git commit -m "你的說明" && git push
```
