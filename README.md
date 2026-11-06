# OmniDoc

OmniDoc 是一款可免费下载使用的桌面办公软件，用于编辑文档、表格、演示文稿和 PDF，也提供免费整篇文档翻译。

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

## 免费文档翻译

在浏览器中打开[免费 PDF 翻译入口](https://omnidoc.top/guides/free-pdf-translator/)，登录后进入「免费翻译」。

上传整篇文件并选择目标语言，等待处理完成后下载结果，不需要逐段复制粘贴。

PDF 与 LaTeX 文件翻译后，双语对照版和纯译文各给一份：前者便于逐段核对，后者适合连续阅读。

翻译时会尽量保留原文件的标题层级、段落、表格和图片位置。

支持 PDF、Word、PowerPoint、Excel、CSV、EPUB、Markdown、TXT、网页、字幕、图片，以及 LaTeX 的 `.tex` 文件和源码包；支持 90 多种语言。

**免费规则**

- 不扣积分。
- 单个文件最多 200 页。
- 每人同时处理 2 个文件，其余排队。
- 每天有免费名额。
- 翻译结果只有提交人自己看得到。

![OmniDoc 双语对照翻译界面](https://omnidoc.top/images/screenshots/zh/translate-bilingual-1280.webp)

上图展示双语对照翻译界面，原文和译文放在一起，便于核对内容。

## 许可与链接

OmniDoc 是专有软件，不是开源软件。本仓库只发布安装包，源代码不公开。软件可免费下载、安装和使用，具体许可见 [LICENSE](LICENSE)。

在线功能（账号、翻译、AI、分享、签署）另受[服务条款](https://omnidoc.top/terms)和[隐私政策](https://omnidoc.top/privacy)约束。

- [官网](https://omnidoc.top/)
- [下载页](https://download.omnidoc.top/)
- [开发者文档](https://docs.omnidoc.top/)
- [免费 PDF 翻译](https://omnidoc.top/guides/free-pdf-translator/)

# OmniDoc (English)

OmniDoc is a free-to-use desktop application for editing documents, spreadsheets, presentations and PDFs. It also offers free translation of entire documents.

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

## Free document translation

Open the [free PDF translator](https://omnidoc.top/guides/free-pdf-translator/) in your browser and sign in. Upload a whole file, choose the target language and download the results when processing finishes.

For PDF and LaTeX files, you receive both a bilingual version for checking against the original and a translation-only version for uninterrupted reading. Translation aims to preserve the original layout, including headings, paragraphs, tables and image positions.

Supported inputs include PDF, Word, PowerPoint, Excel, CSV, EPUB, Markdown, TXT, web pages, subtitles, images, and LaTeX `.tex` files or source bundles. Translation is available in more than 90 languages.

The free service has these limits:

- No credits are deducted.
- Each file can contain up to 200 pages.
- Up to two files per person are processed at once; additional files wait in the queue.
- Free slots are available each day, in limited numbers.
- Only the person who submitted a file can view its translation results.

![OmniDoc bilingual translation interface](https://omnidoc.top/images/screenshots/en/translate-bilingual-1280.webp)

The screenshot shows the bilingual view, with the original text alongside its translation for comparison.

## License and links

OmniDoc is proprietary software, not open source. This repository distributes installers only; the source code is not public. You may download, install and use the software free of charge under the [LICENSE](LICENSE).

Online features—accounts, translation, AI, sharing and signing—are also governed by the [Terms of Service](https://omnidoc.top/terms) and [Privacy Policy](https://omnidoc.top/privacy).

Visit the [website](https://omnidoc.top/) for product information, the [download page](https://download.omnidoc.top/) or [Releases](https://github.com/CBIhalsen/omnidoc/releases) for installers, and the [developer documentation](https://docs.omnidoc.top/) for MCP access. The [free PDF translator](https://omnidoc.top/guides/free-pdf-translator/) requires sign-in.

<sub>仓库只发布安装包；免费翻译需要登录并排队，每天名额有限；AI 译文请对照原文核对重要内容。</sub>
