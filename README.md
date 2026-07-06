# Arabic Bilingual Translator

**Language / 语言 / اللغة:** [中文](#中文) | [English](#english) | [العربية](#العربية)

## 中文

`arabic-bilingual-translator` 是一个面向 Codex 的阿语双语翻译 skill，用于把阿拉伯语、英语或中文来源材料转换成专业的双语 Word 文件，特别适合法律、监管、商务和正式往来文件。

### 基本功能

- 支持 `.docx`、PDF、扫描版 PDF、截图、页面图片和拍照文件。
- 默认生成阿英对照和阿中对照 Word 文件：
  - `EN-AR`：英文在左，阿文在右。
  - `ZH-AR`：中文在左，阿文在右。
- 正确处理阿拉伯语从右到左排版，减少 Word 中常见的文字方向、数字顺序和表格错位问题。
- 保留原文结构，包括标题、编号、条款层级、签名栏、表格、引用编号和法律文书格式。
- 识别法律与通用文本场景，并使用对应术语表。
- 对沙特和 GCC 法律、监管机构、竞争法术语、回历日期和正式称谓提供一致翻译。
- 对扫描件或图片材料提供视觉读取流程，避免直接 OCR 或 PDF 抽取导致的阿文错读。
- 在交付时生成译者说明，标记歧义、不可读区域、日期换算、术语选择和需要律师确认的判断点。

### 适用场景

- 翻译阿语 PDF、扫描件或图片。
- 生成阿英或阿中双栏对照 Word 文件。
- 处理沙特/GCC 法律文件、监管函件、竞争法调查材料、合同、备忘录或正式公文。
- 将英文或中文材料翻译成阿语，并保留双语审阅格式。

### 仓库内容

- `SKILL.md`：skill 的完整工作流和翻译规则。
- `references/`：法律术语表、通用术语表、PDF/图片读取指南、RTL 与日期处理规则。
- `assets/`：生成双语 Word 文件的 `docx-js` 和 `python-docx` 模板。
- `scripts/`：环境检查和 PDF/图片预处理脚本。

> 说明：本 skill 生成的是供律师、业务或合规团队审阅使用的工作译文，不等同于认证翻译或宣誓翻译。

---

## English

`arabic-bilingual-translator` is a Codex skill for producing professional Arabic bilingual translation deliverables from Arabic, English, or Chinese source materials. It is designed especially for legal, regulatory, commercial, and formal documents.

### Core Capabilities

- Supports `.docx`, PDFs, scanned PDFs, screenshots, page images, and photographed documents.
- Produces bilingual Word files by default:
  - `EN-AR`: English on the left, Arabic on the right.
  - `ZH-AR`: Chinese on the left, Arabic on the right.
- Handles Arabic right-to-left rendering correctly in Word, reducing common layout issues with text direction, numbers, and tables.
- Preserves document structure, including headings, numbering, clause hierarchy, signature blocks, tables, reference IDs, and legal formatting.
- Detects legal vs. general translation mode and applies the appropriate glossary.
- Provides consistent renderings for Saudi/GCC legal terms, regulators, competition-law terminology, Hijri dates, and formal honorifics.
- Includes a visual-reading workflow for scanned PDFs and images to avoid silent Arabic misreads from OCR or PDF text extraction.
- Delivers a translator's note that flags ambiguities, unreadable areas, date conversions, terminology choices, and judgment calls for counsel review.

### Typical Use Cases

- Translating Arabic PDFs, scans, screenshots, or photos.
- Creating English-Arabic or Chinese-Arabic side-by-side Word files.
- Handling Saudi/GCC legal documents, regulator letters, competition-law investigation materials, contracts, memoranda, and formal correspondence.
- Translating English or Chinese material into Arabic while preserving a bilingual review format.

### Repository Contents

- `SKILL.md`: the full workflow and translation rules.
- `references/`: legal glossary, general glossary, PDF/image intake guide, and RTL/date handling rules.
- `assets/`: `docx-js` and `python-docx` templates for building bilingual Word files.
- `scripts/`: environment checking and PDF/image preprocessing utilities.

> Note: this skill produces working translations for review by legal, business, or compliance teams. It does not produce certified or sworn translations.

---

## العربية

`arabic-bilingual-translator` هي مهارة مخصصة لـ Codex لإنتاج ترجمات ثنائية اللغة من العربية أو الإنجليزية أو الصينية في ملفات Word احترافية، وهي مناسبة خصوصا للمستندات القانونية والتنظيمية والتجارية والمراسلات الرسمية.

### الوظائف الأساسية

- تدعم ملفات `.docx` وملفات PDF وملفات PDF الممسوحة ضوئيا ولقطات الشاشة وصور الصفحات والمستندات المصورة.
- تنتج افتراضيا ملفات Word ثنائية اللغة:
  - `EN-AR`: الإنجليزية في العمود الأيسر، والعربية في العمود الأيمن.
  - `ZH-AR`: الصينية في العمود الأيسر، والعربية في العمود الأيمن.
- تعالج اتجاه الكتابة العربية من اليمين إلى اليسار داخل Word بطريقة صحيحة، وتقلل مشكلات اتجاه النص والأرقام والجداول.
- تحافظ على بنية المستند الأصلي، بما في ذلك العناوين والترقيم وتسلسل البنود والتوقيعات والجداول وأرقام المراجع والتنسيق القانوني.
- تميز بين النصوص القانونية والعامة وتستخدم قائمة المصطلحات المناسبة لكل حالة.
- توفر ترجمات متسقة لمصطلحات الأنظمة والجهات التنظيمية في السعودية ودول مجلس التعاون، ومصطلحات نظام المنافسة، والتواريخ الهجرية، والألقاب الرسمية.
- تتضمن مسار قراءة بصرية لملفات PDF الممسوحة والصور لتجنب أخطاء OCR أو استخراج النصوص العربية من PDF دون تحقق.
- تضيف ملاحظة مترجم في نهاية التسليم لتوضيح مواضع الغموض، والأجزاء غير المقروءة، وتحويلات التاريخ، واختيارات المصطلحات، والنقاط التي تحتاج إلى مراجعة قانونية.

### حالات الاستخدام

- ترجمة ملفات PDF العربية أو المستندات الممسوحة أو الصور.
- إنشاء ملفات Word ثنائية العمود للعربية والإنجليزية أو العربية والصينية.
- التعامل مع المستندات القانونية السعودية والخليجية، وخطابات الجهات التنظيمية، ومواد تحقيقات المنافسة، والعقود، والمذكرات، والمراسلات الرسمية.
- ترجمة مواد إنجليزية أو صينية إلى العربية مع الحفاظ على صيغة مراجعة ثنائية اللغة.

### محتويات المستودع

- `SKILL.md`: سير العمل الكامل وقواعد الترجمة.
- `references/`: قاموس قانوني، قاموس عام، دليل إدخال ملفات PDF والصور، وقواعد اتجاه النص والتواريخ.
- `assets/`: قوالب `docx-js` و`python-docx` لإنشاء ملفات Word ثنائية اللغة.
- `scripts/`: أدوات فحص البيئة وتجهيز ملفات PDF والصور.

> ملاحظة: تنتج هذه المهارة ترجمة عمل قابلة للمراجعة من الفرق القانونية أو التجارية أو فرق الامتثال، ولا تعد ترجمة معتمدة أو محلفة.
