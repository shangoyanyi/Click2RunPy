# Click2RunPy

為 `.py` 腳本加上右鍵選單，只要點右鍵 → 執行 Python 程式，簡單方便。

---

## 這是什麼？

`Click2RunPy` 是一個小巧的 Windows 工具，透過註冊表檔（`.reg`）讓你的 `.py` 檔在檔案總管中多一個右鍵選單項目：

> 🖱️「用 Python 執行」→ 直接呼叫指定版本的 Python 來執行該腳本。

這特別適合你：
- ✅ 不想每次都開 CMD/PowerShell 跑腳本
- ✅ 有多個 Python 安裝版本，需要手動指定
- ✅ 經常在寫 Python 小工具或自動化腳本

---

## 檔案內容

| 檔案名稱 | 功能說明 |
|----------|----------|
| `Click2RunPy_EnableContextMenu.reg` | ✅ 加入右鍵選單「用 Python 執行」 |
| `Click2RunPy_DisableContextMenu.reg` | ❌ 移除上述右鍵選單 |

---

## ⚠️注意事項

### 修改安裝路徑（必要步驟）

請 **務必打開 `.reg` 檔案**，將裡面的 Python 執行路徑(下面這行)修改為你自己的安裝位置：

```reg
@="\"C:\\Users\\user\\AppData\\Local\\Programs\\Python\\Python313\\python.exe\" \"%1\""
