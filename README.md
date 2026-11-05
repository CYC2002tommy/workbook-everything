# Workbook Everything

把課本、投影片、筆記和考古題丟給 Claude，它會全部讀完，做成一份比較好讀、帶圖解的講義 PDF。

*A Claude Code skill: give it a course's textbook, lecture slides, notes and past exam papers, and it writes one easy-to-read study handout with diagrams.*

## 它怎麼寫

1. **標題是問題**：每一節的標題就是這段在回答的問題，記得問題就推得回答案。
2. **先講機制，再給名詞**：先說誰推誰、為什麼，最後才出現術語。
3. **重點都有圖**：每個重點配一張機制圖，圖上每個形狀都有標籤。
4. **比較一律用表格**。
5. **有考古題時**：每題附原題、拿滿分的最短答和圖，並標出老師常考的、超出範圍的。

## 安裝

```bash
git clone https://github.com/CYC2002tommy/workbook-everything ~/.claude/skills/workbook-everything
```

## 使用

把資料給 Claude，然後說「幫我做講義」或 "make a study handout from these"。

版面細節在 [references/layout.md](references/layout.md)，預設用 XeLaTeX 和 TikZ 出 PDF。

## 授權

MIT
