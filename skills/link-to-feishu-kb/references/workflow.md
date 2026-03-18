# Link → Feishu KB workflow

## Quick checklist

- Open or fetch the source link
- Extract title / source type / core argument
- Decide whether the page is text-rich or media-heavy
- Summarize conservatively
- Create single-item doc
- Add `## 原始链接`
- Search for existing roundup doc
- Reuse if found; otherwise create one
- Append the new entry
- Return both links

## Single-item doc skeleton

```md
<callout emoji="💡" background-color="light-blue">
一句话核心观点
</callout>

## 这篇内容在讲什么

## 核心观点 / 框架

## 值得记住的启发

## 可直接拿去用的清单 / 模板

## 一句话总结

<callout emoji="✅" background-color="light-green">
一句话总结
</callout>

---

## 原始链接

- 原文：[标题](链接)
```

## Roundup doc skeleton

```md
<callout emoji="📚" background-color="light-blue">
这里汇总的是已整理并落地为飞书云文档的内容。
</callout>

## 已整理文档

### 1. 标题
- 文档链接：[点击打开](https://www.feishu.cn/docx/...)
- 原始链接：[原文](https://example.com/...)
- 内容摘要：一句话摘要
```

## Roundup update rules

- Preserve the existing roundup title when one already exists.
- Append one new block per source unless the user explicitly asks for reordering or deduplication.
- If an existing roundup is topic-specific, keep new entries stylistically consistent with it.
- Return both the single-item doc link and the roundup doc link.
