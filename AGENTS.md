# Repository Guidelines

## Project Structure & Module Organization
The root folder `璁烘枃寮€棰榒 holds faculty notices (for example `2025骞寸瀛︽湡寮€棰橀€氱煡.pdf`) and the source archives. All editable forms live inside `寮€棰樼浉鍏宠〃鏍?璇峰悓瀛﹁鐪熼槄璇汇€佸～鍐?/(寮€棰樼浉鍏宠〃鏍?璇峰悓瀛﹁鐪熼槄璇汇€佸～鍐?)`, where you will find Word templates such as `璇鹃缁勭爺绌剁敓瀛︽湳娲诲姩璁板綍琛?doc` and `棰樼洰鐢虫姤鏍煎紡瑕佹眰.doc`. Keep original downloads untouched; add personalized drafts alongside the templates rather than renaming the directories.

## Build, Test, and Development Commands
Open documents with Microsoft Word or WPS:  
`start "" "寮€棰樼浉鍏宠〃鏍?璇峰悓瀛﹁鐪熼槄璇汇€佸～鍐?\寮€棰樼浉鍏宠〃鏍?璇峰悓瀛﹁鐪熼槄璇汇€佸～鍐?\棰樼洰鐢虫姤鏍煎紡瑕佹眰.doc"`.  
To export a PDF from Word via PowerShell, run `Start-Process winword.exe "/mFileSaveAsPDF \"$(Resolve-Path .\鑽夌.docx)\""` after enabling the macro. Always place generated PDFs next to their source DOC/DOCX files so reviewers can trace revisions.

## Coding Style & Naming Conventions
Write content in simplified Chinese, using Songti body text, 1.5 line spacing, and the heading hierarchy defined in each template. Save drafts as `YYYYMMDD-涓婚-鐗堟湰.docx` (e.g., `20251028-寮€棰樻姤鍛?v1.docx`) to keep chronological order. Track reviewer input with Word鈥檚 comment feature; avoid inline colors. Before committing, strip personal IDs, signatures, and stamps from template copies.

## Testing Guidelines
Run Word鈥檚 鈥滄嫾鍐欏拰璇硶妫€鏌モ€?and compare changes with the previous version (`瀹￠槄 鈫?姣旇緝`) before exporting. After producing the PDF, confirm that tables, signatures, and embedded images render correctly and that margins match the faculty specification. When attachments reference external evidence, verify the hyperlinks or annex numbers.

## Commit & Pull Request Guidelines
Use concise prefixes in commit subjects (`docs:`, `forms:`, `ref:`) followed by the main update, e.g., `docs: refresh 寮€棰樻姤鍛婃ā鐗?wording`. A pull request should include: (1) a summary of the modifications, (2) a checklist of updated files with their statuses (draft/final), (3) confirmation that spell-check and PDF export passed, and (4) links to meeting minutes or department tickets. Attach screenshots only when layout changes are non-trivial; exclude binary previews from Git history.

## Security & Data Handling
Store signed or personal-information versions outside the repository and add their filenames to `.gitignore`. When sharing deliverables, compress them with a password that follows faculty policy. Delete any cached comparison files after review to prevent accidental disclosure.

## Active Thesis Topic
- 课题名称：涉虚拟货币洗钱犯罪监管体系的协同治理研究（MPA 硕士开题）
- 当前状态：已与导师确认选题，可据此撰写开题报告与相关材料。

