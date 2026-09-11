---
title: Test Blog 
math: true
mermaid: true
date: 2026-09-11
categories: 环境搭建
---

<!--more-->

## 数学公式

行内公式 $a+b=c$

行间公式
$$
a^2 + b^2 = c^2
$$

## 字体

英文示例: Best wishes for you!

中文示例: 落霞与孤鹜齐飞，秋水共长天一色。

## mermaid 流程图

```mermaid
graph TD
    A["Part 1: 单脉冲 LFM 回波信号建模与加噪"] --> B["Part 2: 相控阵空间接收、和差波束形成与理论鉴角特性"]
    B --> C["Part 3: 和差波束时域合成与相关能量累积比值提取"]
    C --> D["Part 4: 目标角度估计解算"]
```

## 代码块

单行代码样式：`composer require --dev barryvdh/laravel-ide-helper`

大段代码块样式：

```css
body {
  font-size: 16px;  /* comment */
}
```

```html
<a href="/about.html">Example</a>  <!-- comment -->
```

```go-html-template
{{ with $.Page.Params.content }}
  {{ . | $.Page.RenderString }}  {{/* comment */}}
{{ end }}
```

```javascript
if ([1,"one",2,"two"].includes(value)){
  console.log("Number is either 1 or 2.");  // comment
}
```

```toml
[params]
bool = true  # comment
string = 'foo'
```

## 盘古之白

你好, 我的英文名字是Zhanghua, 今年18岁.
