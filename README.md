# OmniDoc

OmniDoc 是一款可免费下载使用的桌面办公软件，用于编辑文档、表格、演示文稿和 PDF，也提供免费整篇文档翻译和免费结构化提取。

[官网](https://omnidoc.top/) · [English](#omnidoc-english)

## 下载

当前版本：**OmniDoc 1.09 build 131**。

| 系统 | 安装包 | 大小 | SHA-256 |
| --- | --- | --- | --- |
| Windows 10 / 11（64 位） | `OmniDoc-1.09-b131-Windows-x64-Setup.exe` | 312,273,512 字节 | `b1e2b4e15ae573aed622d5dcdf2e7a42ef1e5c7002e2ec6b24c3769b632b5a53` |
| Linux x86_64（Ubuntu、Debian 等） | `OmniDoc-1.09-b131-Linux-x86_64.deb` | 390,399,672 字节 | `2f037efec0d978d61152c0078b3f95d740cc767085ac634eb6d3b5adfb1f7cde` |
| macOS 12 及以上（Intel） | `OmniDoc-1.09-b131-macOS-x64.dmg` | 362,695,549 字节 | `ee85444969c30e79cc7b82608184926d39af8582d4e7c7f1537e10b036c7b888` |

安装包在 [Releases](https://github.com/CBIhalsen/omnidoc/releases) 和[官网下载页](https://download.omnidoc.top/)提供。下载后可用上表的 SHA-256 核对文件。

## 办公能力

在桌面版中，可以直接编辑常见办公文件：

- **文档**：修改正文、章节结构、样式和表格，调整页面排版。
- **表格**：处理多张工作表、公式、条件格式和图表。
- **演示文稿**：编辑幻灯片内容、表格、图表和备注。

编辑 PDF 时，可以点进段落直接改字；打字时显示的就是保存后的排版。

PDF 工具还包括电子签名、表单和文字识别，并支持导出为 Word、Excel、PowerPoint，方便继续编辑。

通过 AI 接口 **MCP**，Claude、Codex、Cursor 等可以直接读取、编辑和导出文档。打开着的文档会跟着 AI 的修改原地更新，可以在窗口中查看修改结果。

接入方式见[开发者文档](https://docs.omnidoc.top/)。

## 流畅、Office 原生格式和中文国标格式

- **打开快、保存快**：13.6 MB 的论文 PDF 从启动到显示第一页约 4 秒，保存约 0.06 秒；在 PDF 段落里打字，页面直接显示最终排版，写回一个段落约 0.3 秒；文档编辑器从按键到排好版约 9 毫秒。
- **原生读写 Word、Excel、PowerPoint**：.docx、.xlsx、.pptx 直接打开、直接保存，存出来仍是标准的 Office Open XML 文件。Word 的内容控件、书签、分页符、页眉页脚和脚注原样保留；Excel 的公式、原生图表、数据透视表、条件格式、筛选和迷你图照常工作。
- **中文国标格式**：OFD 版式文件（GB/T 33190）可以直接打开、编辑和另存，PDF 与 OFD 互相转换；中文期刊论文模板按 GB/T 7714—2015 著录参考文献，学位论文模板按 GB/T 7713.1 排版；多级编号自带公文层级：一、（一）1.（1）。

## 免费文档翻译

在浏览器中打开[免费文档翻译](https://omnidoc.top/free/translate/)，用 OmniDoc 账号登录（注册免费），不需要安装软件。

上传整篇文件，原文语言自动识别，选择目标语言后等待处理完成再下载，不需要逐段复制粘贴。关闭页面不影响处理，之后可在「最近的翻译」里找到结果。

PDF 与 LaTeX 文件翻译后，双语对照版和纯译文各给一份：前者便于逐段核对，后者适合连续阅读。PowerPoint 只提供纯译文。

翻译时会尽量保留原文件的标题层级、段落、表格和图片位置；表格逐格翻译，行列结构不变。

支持 PDF、Word、PowerPoint、Excel、CSV、EPUB、Markdown、TXT、HTML、SRT/ASS 字幕、JPG/PNG 图片，以及 LaTeX 的 `.tex` 文件和源码包；可译为中文、英文、日文、韩文、法文、德文、西班牙文等 30 多种语言。

**免费规则**

- 需要登录，注册免费。
- 单个文件最多 501 页。
- 每人同时处理 2 个文件，其余按提交顺序排队。
- 上传的文件和处理结果只有提交人自己看得到。
- 免费翻译采用机器翻译，重要文件请核对数字、术语和引用。

![OmniDoc 双语对照翻译界面](https://omnidoc.top/images/screenshots/zh/translate-bilingual-v2-1280.webp)

上图展示双语对照翻译界面，原文和译文放在一起，便于核对内容。

## 免费结构化提取

在浏览器中打开[免费结构化提取](https://omnidoc.top/free/extract/)，登录后上传 PDF、扫描件、Word、PowerPoint 或 Excel 文件，得到 Markdown 和 JSON。

PDF、扫描件和图片经版面分析、文字识别和表格识别处理；Word、PowerPoint、Excel、电子书和网页直接解析文档结构。下载的 ZIP 压缩包里有 `document.md`（Markdown 全文）、`document.json`（按阅读顺序排列的结构化数据）、`images/`（文档中的图片）和 `manifest.json`（文件清单）。

标题层级、段落和表格行列都会保留。PDF 单个文件最多 501 页，每人同时处理 2 个文件。扫描件的识别结果请与原文核对，尤其是数字和表格。

## 常见问题

**怎么翻译 PDF 又不乱版？**
打开[免费文档翻译](https://omnidoc.top/free/translate/)，登录后上传 PDF。OmniDoc 整篇翻译，标题、段落、表格（逐格翻译）、公式和图片放回原位，同时给出双语对照版和纯译文版。免费版单个文件最多 501 页。

**LaTeX 论文、arXiv 源码包能翻译吗？**
能。上传 `.tex` 文件或整个源码包，公式原样保留，输出双语对照版和纯译文版。

**扫描版 PDF 怎么转成 Markdown 或 JSON？**
用[免费结构化提取](https://omnidoc.top/free/extract/)：扫描件先做文字识别，再按版面整理标题、段落和表格，下载的 ZIP 里有 `document.md`、`document.json` 和图片。

**Claude、Cursor 能用 OmniDoc 直接改 Word、Excel、PPT 吗？**
能。桌面版自带 MCP 服务，40 多个文档工具；AI 在你的电脑上新建、修改和导出文件，编辑和格式转换离线免费，翻译等云端服务按积分计费，不需要 API Key。接入方式见[开发者文档](https://docs.omnidoc.top/)。

**OmniDoc 开源吗？**
不开源。OmniDoc 是专有软件，可以免费下载、安装和使用，许可见 [LICENSE](LICENSE)。

## 许可与链接

OmniDoc 是专有软件，不是开源软件。本仓库只发布安装包，源代码不公开。软件可免费下载、安装和使用，具体许可见 [LICENSE](LICENSE)。

在线功能（账号、翻译、AI、分享、签署）另受[服务条款](https://omnidoc.top/terms)和[隐私政策](https://omnidoc.top/privacy)约束。

- [官网](https://omnidoc.top/)
- [下载页](https://download.omnidoc.top/)
- [开发者文档](https://docs.omnidoc.top/)
- [免费文档翻译](https://omnidoc.top/free/translate/)
- [免费结构化提取](https://omnidoc.top/free/extract/)

# OmniDoc (English)

OmniDoc is a free-to-use desktop application for editing documents, spreadsheets, presentations and PDFs. It also offers free translation of entire documents and free structured extraction.

[Website](https://omnidoc.top/) · [Downloads](https://download.omnidoc.top/) · [Developer documentation](https://docs.omnidoc.top/)

## Download

The current release is **OmniDoc 1.09 build 131**, available for Windows (`.exe`), Linux (`.deb`) and macOS (`.dmg`). Get the installers from [GitHub Releases](https://github.com/CBIhalsen/omnidoc/releases) or the [download page](https://download.omnidoc.top/).

The [download table above](#下载) lists the supported systems, exact filenames, file sizes and SHA-256 checksums for all three packages.

## Editing and AI access

Use OmniDoc to work on the files themselves:

- **Documents:** edit text, headings, styles, tables and page layout.
- **Spreadsheets:** work with multiple sheets, formulas, conditional formatting and charts.
- **Presentations:** edit slide content, tables, charts and speaker notes.

For PDFs, click into a paragraph and type. The layout you see as you edit is the layout saved to the file. PDF tools also include electronic signatures, forms, text recognition and export to Word, Excel and PowerPoint.

The **MCP interface** gives AI assistants such as Claude, Codex and Cursor direct access to read, edit and export documents. If a document is open in OmniDoc, the AI's changes appear in that same window as it works. See the [developer documentation](https://docs.omnidoc.top/) for connection instructions.

## Speed, native Office formats and Chinese standard formats

- **Quick to open and save:** a 13.6 MB research paper in PDF shows its first page about 4 seconds after launch and saves in about 0.06 seconds. Type into a PDF paragraph and the page shows the final layout as you type; writing the paragraph back takes about 0.3 seconds. In the document editor a key press is laid out in about 9 milliseconds.
- **Word, Excel and PowerPoint, read and written natively:** .docx, .xlsx and .pptx files open and save directly and stay standard Office Open XML files. Word content controls, bookmarks, page breaks, headers, footers and footnotes are kept; Excel formulas, native charts, pivot tables, conditional formatting, filters and sparklines keep working.
- **Chinese standard formats:** OFD files (GB/T 33190) open, edit and save as they are, and convert to and from PDF. The Chinese journal paper template formats references to GB/T 7714—2015, the thesis template follows GB/T 7713.1, and multilevel numbering includes the official-document levels 一、（一）1.（1）.

## Free document translation

Open the [free document translator](https://omnidoc.top/free/translate/) in your browser and sign in with an OmniDoc account (registration is free); nothing needs to be installed. Upload a whole file and the source language is detected for you. Choose the target language and download the results when processing finishes.

For PDF and LaTeX files, you receive both a bilingual version for checking against the original and a translation-only version for uninterrupted reading; PowerPoint comes back as translation-only. Translation aims to preserve the original layout, including headings, paragraphs, tables (translated cell by cell) and image positions.

Supported inputs include PDF, Word, PowerPoint, Excel, CSV, EPUB, Markdown, TXT, HTML, SRT and ASS subtitles, JPG and PNG images, and LaTeX `.tex` files or source bundles. Target languages include Chinese, English, Japanese, Korean, French, German and Spanish, 30+ in total.

The free service has these limits:

- Sign-in is required; registration is free.
- Each file can contain up to 501 pages.
- Up to two files per person are processed at once; additional files wait in the queue in the order they were submitted.
- Only the person who submitted a file can view its results.
- It is machine translation: please check numbers, terms and citations in important documents.

![OmniDoc bilingual translation interface](https://omnidoc.top/images/screenshots/en/translate-bilingual-v2-1280.webp)

The screenshot shows the bilingual view, with the original text alongside its translation for comparison.

## Free structured extraction

Open the [free structured extractor](https://omnidoc.top/free/extract/) in your browser, sign in, and upload a PDF, scan, Word, PowerPoint or Excel file to get Markdown and JSON.

PDFs, scans and images go through layout analysis, OCR and table recognition. Word, PowerPoint, Excel, EPUB and HTML files are parsed directly. The downloaded ZIP contains `document.md` (the full text as Markdown), `document.json` (structured data in reading order), `images/` (the pictures) and `manifest.json` (a file list).

Heading levels, paragraphs and table rows and columns are kept. Up to 501 pages per PDF and two files at a time. Please check OCR results against the original, especially numbers and tables.

## Frequently asked questions

**How do I translate a PDF without losing the layout?**
Open the [free document translator](https://omnidoc.top/free/translate/), sign in and upload the PDF. OmniDoc translates the whole file and puts headings, paragraphs, tables (translated cell by cell), formulas and images back where they were, and returns a bilingual version and a translation-only version. The free service takes files of up to 501 pages.

**Can I translate a LaTeX paper or an arXiv source package?**
Yes. Upload the `.tex` file or the whole source bundle; formulas are kept as written, and you get a bilingual and a translation-only version.

**How do I convert a scanned PDF to Markdown or JSON?**
Use the [free structured extractor](https://omnidoc.top/free/extract/). Scans go through text recognition, then headings, paragraphs and tables are rebuilt from the layout. The ZIP contains `document.md`, `document.json` and the images.

**Can Claude or Cursor edit Word, Excel and PowerPoint files with OmniDoc?**
Yes. The desktop app includes an MCP server with more than 40 document tools. Your assistant creates, edits and exports files on your computer; editing and conversion are offline and free, and cloud services such as translation use credits. No API key is needed. See the [developer documentation](https://docs.omnidoc.top/).

**Which systems are supported?**
Windows 10 and 11 (x64), macOS 12 or later (Intel) and 64-bit Linux distributions based on Debian (glibc 2.30 or later), such as Ubuntu 20.04 and Debian 11.

**Is OmniDoc open source?**
No. OmniDoc is proprietary software that you can download, install and use free of charge under the [LICENSE](LICENSE).

## License and links

OmniDoc is proprietary software, not open source. This repository distributes installers only; the source code is not public. You may download, install and use the software free of charge under the [LICENSE](LICENSE).

Online features—accounts, translation, AI, sharing and signing—are also governed by the [Terms of Service](https://omnidoc.top/terms) and [Privacy Policy](https://omnidoc.top/privacy).

Visit the [website](https://omnidoc.top/) for product information, the [download page](https://download.omnidoc.top/) or [Releases](https://github.com/CBIhalsen/omnidoc/releases) for installers, and the [developer documentation](https://docs.omnidoc.top/) for MCP access. The [free translator](https://omnidoc.top/free/translate/) and [free extractor](https://omnidoc.top/free/extract/) require sign-in.

<sub>仓库只发布安装包；免费翻译和免费提取需要登录，文件较多时需要排队；AI 译文和识别结果请对照原文核对重要内容。</sub>
