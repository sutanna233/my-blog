---
title: 'Astro 学习笔记'
description: '记录学习 Astro 框架的过程和心得。'
pubDate: '2024-01-20'
heroImage: '/blog-placeholder-2.jpg'
categories: ['技术']
tags: ['Astro', '前端', '学习笔记']
---

# Astro 学习笔记

Astro 是一个专注于内容的静态站点生成器，它的设计理念是"默认零 JavaScript"。

## 核心特性

### 1. Islands Architecture

Astro 采用 Islands 架构，允许你只对需要交互的部分使用 JavaScript：

```astro
<MyComponent client:load />
```

### 2. 内容集合

使用内容集合来管理 Markdown 文件：

```typescript
import { defineCollection, z } from 'astro:content';

const blog = defineCollection({
  schema: z.object({
    title: z.string(),
    pubDate: z.coerce.date(),
  }),
});
```

### 3. 组件化

Astro 支持多种 UI 框架的组件，包括 React、Vue、Svelte 等。

## 学习资源

- [Astro 官方文档](https://docs.astro.build)
- [Astro 中文网](https://astro.js.cn)

继续探索中...
