# RMT Blog

Guide for local Hexo debugging and adding new documentation posts.

## Prerequisites

- Node.js LTS and npm installed
- Git installed
- Hexo CLI (optional for global use)

```bash
npm install -g hexo-cli
```

## Local Development (Debug)

1. Install dependencies in the repository root:

```bash
npm install
```

2. Start the local server:

```bash
npm run server
```

3. Open the site in your browser:

```text
http://localhost:4000
```

4. (Optional) Clean cache if you see stale content:

```bash
npx hexo clean
```

## Deploy to Github Pages

Trigger the pages workflows in Actions.

## Add a New Documentation Post

This repository stores posts under `source/_posts/<locale>/`. Create the
Markdown file in the target locale folder and follow the front-matter format.

### Step 1: Create the Markdown file

Example paths:

- `source/_posts/en-US/your-doc-title.md`
- `source/_posts/zh-CN/your-doc-title.md`

### Step 2: Add front matter

Use a YAML front matter block at the top of the file:

```yaml
---
title: "Your Doc Title"
date: 2026-02-09 10:00:00
tags:
	- docs
categories:
	- documentation
---
```

### Step 3: Write content

Add your Markdown content below the front matter. Use headings, lists, and code
blocks as needed.

### Step 4: Preview locally

```bash
npx hexo server --draft
```

## Publish (Generate Static Files)

```bash
npx hexo generate
```
