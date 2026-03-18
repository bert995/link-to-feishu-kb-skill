# link-to-feishu-kb

Turn public links into structured Feishu knowledge docs and keep a running roundup page updated.

This skill is designed for the workflow where you drop in a link — a Xiaohongshu post, blog post, company article, essay, or documentation page — and want the agent to do the whole loop in one pass:

1. read the source conservatively
2. create a structured summary
3. create a Feishu cloud doc for the single item
4. append the result to an existing roundup/index doc

## What it supports

- Xiaohongshu / Rednote links
- public articles and essays
- product / engineering blog posts
- documentation-style pages

## Default workflow

1. Read the source link and extract supported facts only.
2. Identify the source type.
3. Produce a structured summary rather than a fake transcript.
4. Create a single-item Feishu doc titled `<原标题>｜内容汇总`.
5. Add a `## 原始链接` section in the single-item doc.
6. Search for an existing roundup doc and reuse it when possible.
7. Append a new entry with:
   - title
   - generated Feishu doc link
   - original source link
   - one-line summary

## Output

The skill returns:
- a single-item Feishu doc link
- a roundup/index doc link

The single-item doc is usually organized as:
- core thesis
- what the source is about
- key ideas / arguments
- practical takeaways
- reusable checklist or template when useful
- original source link

## Repo layout

```text
skills/
  link-to-feishu-kb/
    SKILL.md
    references/
      workflow.md
      source-types.md
      github-skills-md.md
```

## Notes

- The skill prefers honest structured summaries over pretending to have a full transcript.
- If a page is partially accessible, it summarizes only what can actually be read.
- If a topic-specific roundup doc already exists, it reuses that instead of silently creating another one.

## Example prompts

- “把这个小红书链接整理成飞书文档，并加入汇总页。”
- “这个 OpenAI 文章按我们之前那个 skill 走一下。”
- “把这篇工程博客整理进我的知识库。”
