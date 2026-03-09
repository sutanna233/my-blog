---
title: 'Tailwind CSS 实用技巧'
description: '分享一些 Tailwind CSS 的使用技巧和最佳实践。'
pubDate: '2024-01-25'
heroImage: '/blog-placeholder-3.jpg'
categories: ['技术']
tags: ['Tailwind', 'CSS', '前端']
---

# Tailwind CSS 实用技巧

Tailwind CSS 是一个功能类优先的 CSS 框架，下面分享一些实用技巧。

## 1. 暗黑模式

使用 `dark:` 前缀轻松实现暗黑模式：

```html
<div class="bg-white dark:bg-gray-900">
  <h1 class="text-gray-900 dark:text-white">Hello</h1>
</div>
```

## 2. 自定义配置

在 `tailwind.config.mjs` 中自定义主题：

```javascript
export default {
  theme: {
    extend: {
      colors: {
        primary: '#...',
      },
    },
  },
}
```

## 3. 响应式设计

Tailwind 的响应式前缀：

- `sm:` - 640px+
- `md:` - 768px+
- `lg:` - 1024px+
- `xl:` - 1280px+

## 4. 组合类

使用 `@apply` 组合常用样式：

```css
.btn-primary {
  @apply px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600;
}
```

## 5. 动态类名

在需要动态生成类名时使用 `clsx` 或 `tailwind-merge` 库。

希望这些技巧对你有帮助！
