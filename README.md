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

---

## Structure / 目录结构

```
booksofAiEra/
├── books/
│   ├── intelligence-age/     # Book: The Intelligence Age
│   └── crossroads/           # Book: The Crossroads
│       ├── en/               # English edition (mdBook project)
│       │   ├── book.toml
│       │   └── src/
│       └── zh/               # Chinese edition (mdBook project)
│           ├── book.toml
│           └── src/
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
