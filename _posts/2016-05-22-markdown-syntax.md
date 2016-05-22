---
layout: post
title:  "Markdown语法记录"
date:   2016-05-22
excerpt: "今天发现一个markdown语法，之前的没有看到过，以后发现的也一同记录在这里"
tag:
- Markdown 
comments: true
---

>[Markdown语法参考](https://github.com/younghz/Markdown)

## 给链接添加class,注意写在行首

```markdown
[test](# "test"){: .testlink}	-->		<a href="#" class="testlink">test</a>
```
如:

[test](# "test"){: .testlink}

## 给图片添加class,注意写在行首

```markdown
![test](/assets/img/tx.png){: .btn}	-->		<p><img src="/assets/img/tx.png" alt="test" class="btn"></p>
```

如：

![test](/assets/img/tx.png){: .btn}

## 直接插入html,注意写在行首

```html
<div class="ssds" style="border: 1px solid red">这是一个div</div>
```

如：

<div class="ssds" style="border: 1px solid red">这是一个div</div>
