# Books of AI Era

> **宗：Human Wisdom · 以人驭智**
> *Humanity at the center, intelligence as the instrument.*
> *以人为本，智能为用。*

A collection of living field guides to the AI era — continuously updated in English and Chinese.

一系列持续更新的 AI 时代实地指南——中英双语同步更新。

---

## Read / 阅读

| The Intelligence Age | 🇬🇧 English | https://treelemon.github.io/booksofAiEra/intelligence-age/en/ |
|----------------------|-------------|--------------------------------------------------------------|
| 智能时代 | 🇨🇳 中文 | https://treelemon.github.io/booksofAiEra/intelligence-age/zh/ |
| The Crossroads: AI, Education, and the Next Generation | 🇬🇧 English | https://treelemon.github.io/booksofAiEra/crossroads/en/ |
| 十字路口：AI时代的教育与选择 | 🇨🇳 中文 | https://treelemon.github.io/booksofAiEra/crossroads/zh/ |
| 周期之轮：经济波动的底层逻辑、实证测度与决策框架 | 🇨🇳 中文 | https://treelemon.github.io/booksofAiEra/cycles/zh/ |
| 穿越周期：商业银行的命运、逻辑与生存法则 | 🇨🇳 中文 | https://treelemon.github.io/booksofAiEra/bank-and-cycles/zh/ |
| 三驾马车：财富管理、科技金融与跨境金融——银行业未来确定性机会 | 🇨🇳 中文 | https://treelemon.github.io/booksofAiEra/three-carriages/zh/ |
| 周期之眼：信息产业与AI的演进逻辑与投资框架 | 🇨🇳 中文 | https://treelemon.github.io/booksofAiEra/cycles-of-ai-era/zh/ |
| 封锁与突围：中国芯片产业的血色长征 | 🇨🇳 中文 | https://treelemon.github.io/booksofAiEra/silicon-blockade/zh/ |
| 浪潮之轮：技术革命、行业轮动与结构性行情的两百年 | 🇨🇳 中文 | https://treelemon.github.io/booksofAiEra/waves-of-change/zh/ |

---

## Structure / 目录结构

```
booksofAiEra/
├── books/
│   ├── intelligence-age/     # Book: The Intelligence Age
│   ├── crossroads/           # Book: The Crossroads
│   ├── cycles/               # Book: 周期之轮
│   ├── bank-and-cycles/      # Book: 穿越周期（商业银行与经济周期）
│   └── three-carriages/      # Book: 三驾马车（财富管理、科技金融、跨境金融）
│       └── zh/               # Chinese edition
│           ├── book.toml
│           └── src/
├── cycles-of-ai-era/         # Book: 周期之眼（信息产业与AI的演进逻辑与投资框架）
│   └── zh/
│       ├── book.toml
│       └── src/
├── silicon-blockade/         # Book: 封锁与突围（中国芯片产业的血色长征）
│   └── zh/
│       ├── book.toml
│       └── src/
├── waves-of-change/          # Book: 浪潮之轮（技术革命、行业轮动与结构性行情）
│   └── zh/
│       ├── book.toml
│       └── src/
├── .github/workflows/deploy.yml
├── README.md
└── CHANGELOG.md
```

Each book under `books/` contains language-specific mdBook projects with identical structure.

每本书位于 `books/` 目录下，包含各语言的独立 mdBook 项目，结构完全一致。

To add a new book:
```
mkdir -p books/<book-name>/en/src books/<book-name>/zh/src
# ... create book.toml and content for each language
# Then add links to .github/workflows/deploy.yml
```

---

**Status:** Active development · [CHANGELOG](CHANGELOG.md)
