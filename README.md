# GitHub Pages Update Log
ideaHub - HTML/CSS

**04/07**
post-template.html 建立完成。

往後新增文章的流程：

複製 post-template.html → 改名為 post3.html、post4.html...
改 ①②③④ 四個標記處

在內文裡填入.keywords 積木
在 index.html 加一張 .post-card

(本地端先瀏覽../ideaHub/postX.html)

---
**04/08**
把HTML+CSS 框架整個當成 template 檔

測試轉檔工具：
- 輸入：任意 .md 檔案
- 輸出：完整的 .html 檔案（把 MD 轉成 HTML 內容後，塞進 template 的 <article> 或指定區塊）
- 要支援：Markdown 標題、圖片、程式碼區塊、表格、內嵌 YouTube 等
- 使用 markdown + jinja2（或 beautifulsoup）實現
- 加上簡單的 CLI：python md_to_html.py input.md output.html
- 請輸出完整可直接執行的程式碼

把 AI 給的程式碼存成 md_to_html.py，

使用前一次設定（只需執行一次）：
pip install markdown jinja2 beautifulsoup4

每天使用超簡單：
python md_to_html.py 今天文章.md 今天文章.html

---
**04/09**
日誌顯示 Jekyll 正在嘗試渲染你的 Markdown 檔案（例如 Apple_PLM_Truth.md），但可能因為某些格式或佈局設定與 Jekyll 的預設主題不相容而導致編譯中斷。

既然你已經寫好了完整的 HTML，最快速且徹底的解決方案如下：

解決方法：強制跳過 Jekyll 編譯（最推薦）
既然你使用的是自己寫的 index.html 和 style.css，你並不需要 Jekyll 幫你轉檔。請依照以下步驟操作：

建立一個新檔案： 在你的 GitHub 專案根目錄下（與 index.html 同一層），建立一個檔案。

命名為： .nojekyll（注意前面有一個點，且沒有任何副檔名）。

---
**04/10**
新增分頁：所有文章、關於我
修改index文章卡片超連結按鈕範圍 (整張卡片)
