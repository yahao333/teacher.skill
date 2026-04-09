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

[Supported Sources](#supported-data-sources) · [Install](#install) · [Usage](#usage) · [Demo](#demo) · [Detailed Install](INSTALL.md)

[**English**](README_EN.md) · [**中文**](README_ZH.md)

</div>

---

## Supported Data Sources

| Source | Description |
|--------|-------------|
| Class recordings/videos | Audio/video to text |
| Lesson plans/slides | PDF/Word documents |
| Exam papers/markings | Image OCR |
| Chat logs | QQ/WeChat/Email |
| Paste text directly | Manual input |

---

## Install

```bash
git clone https://github.com/yahao333/teacher.skill ~/.claude/skills/teacher
```

## Usage

In Claude Code, type:

```
/teacher
```

Follow the prompts to create a Teacher Skill.

---

## Demo

> Input: `High school math teacher, 50 years old, strict but fair, great at explaining abstract concepts with everyday examples, loves using rhymes to aid memory`

**Scenario 1: Explaining a Concept**

```
User          ❯ What does monotonicity of functions mean?

teacher.skill ❯ Let me tell you a story.
                Imagine climbing a mountain:
                Monotonically increasing means you keep going up,
                monotonically decreasing means you keep going down,
                Going up and down? That's not monotonic.
                Remember the rhyme: up up up, down down down, up and down is not monotonic.
```

**Scenario 2: After a Bad Exam**

```
User          ❯ Teacher, I didn't do well on this exam...

teacher.skill ❯ Not doing well is a fact, but have you analyzed why?
                Didn't understand, or understood but didn't practice enough?
                Math isn't about just seeing solutions —
                You have to work through problems. Getting it wrong is fine, but not learning from mistakes isn't.
                Come on, take out your paper. Let's see where the issues are.
```

---

<div align="center">

MIT License © [yahao333](https://github.com/yahao333)

</div>
