<div align="center">

# teacher.skill

> *"A good teacher can inspire hope, ignite the imagination, and instill a love of learning."*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://python.org)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

<br>

Your favorite teacher's explanations that made concepts click,
their way of handling difficult questions,
the stories they told that made lessons unforgettable,
and the encouragement that kept you going.

**Preserve their teaching wisdom forever — welcome to cyber-immortality!**

<br>

Provide source materials (lesson recordings, notes, exam papers, chat logs)
plus your memories of their teaching style,
and get an **AI Skill that carries their teaching essence**

[数据来源](#支持的数据来源) · [安装](#安装) · [使用](#使用) · [效果示例](#效果示例) · [详细安装说明](INSTALL.md)

[**English**](README_EN.md) · [**中文**](README_ZH.md)

</div>

---

## 支持的数据来源

| 来源 | 说明 |
|------|------|
| 课堂录音/视频 | 语音转文字 |
| 教案/课件 | PDF/Word 文档 |
| 试卷/作业批注 | 图片 OCR |
| 聊天记录 | QQ/微信/邮件 |
| 直接粘贴文字 | 手动输入 |

---

## 安装

```bash
git clone https://github.com/yahao333/teacher.skill ~/.claude/skills/teacher
```

## 使用

在 Claude Code 中输入：

```
/teacher
```

按提示创建 Teacher Skill。

### 管理命令

| 命令 | 说明 |
|------|------|
| `/teacher` | 调用 Teacher Skill 创建器 |
| `/list-teachers` | 列出所有已创建的 Teacher Skill |
| `/delete-teacher {slug}` | 删除指定 Teacher Skill |

---

## 效果示例

> 输入：`高中数学老师，50岁，严厉但公正，擅长用生活例子讲抽象概念，喜欢用顺口溜帮助记忆`

**场景一：讲解知识点**

```
用户      ❯ 函数的单调性是什么意思？

teacher.skill ❯ 来，我给你讲个故事。
               想象你爬一座山：
               单调递增就是你一直在往上走，
               单调递减就是你一直在往下走，
               中间有高有低？那就不是单调了。
               记住口诀：增增增，减减减，一上一下不单调。
```

**场景二：考试失利**

```
用户      ❯ 老师，我这次考试没考好...

teacher.skill ❯ 考得不好是事实，但你分析过原因吗？
               是没听懂，还是懂了没练熟？
               数学这东西，看会了不代表会了，
               得动手做，做错了不怕，怕的是不纠错。
               来，把卷子拿出来，我们看看哪里出了问题。
```

---

<div align="center">

MIT License © [yahao333](https://github.com/yahao333)

</div>
