---
name: teacher
description: "Distill a teacher's explanation style, teaching methods, and educational wisdom into an AI Skill. | 蒸馏老师的教学风格、讲解方法和教育智慧到一个 AI Skill 中。"
argument-hint: "[teacher-name-or-slug]"
version: "1.0.0"
user-invocable: true
allowed-tools: Read, Write, Edit, Bash
---

# 老师.skill 创建器（Claude Code 版）

## 触发条件

当用户说以下任意内容时启动：
- `/teacher`
- "帮我创建一个老师 skill"
- "我想蒸馏老师"
- "新建老师"
- "给我做一个老师的 skill"

---

## 主流程：创建新老师 Skill

### Step 1：基础信息录入

问 3 个问题：

1. **称呼**（必填）：你平时怎么称呼她/他？如「老师」「张老师」「李老师」
2. **基本信息**（一句话）：教什么学科、教哪个年龄段、性格特点
   - 示例：`高中数学老师，40岁，严厉但公平，喜欢用生活中的例子讲解`
3. **特别风格**（可选）：他/她最标志性的教学风格、口头禅或习惯

### Step 2：原材料导入

询问用户提供原材料：

```
原材料怎么提供？

  [A] 课堂录音/视频
      录制讲解某个知识点的片段

  [B] 教案/课件
      备课文档、PPT、习题讲解

  [C] 试卷/作业批注
      手写批改痕迹、评语

  [D] 聊天记录
      与老师的微信/QQ 等沟通记录

  [E] 直接粘贴
      复制文字粘贴进来

可以混用，也可以跳过（仅凭手动信息生成）。
```

### Step 3：分析生成

将收集到的材料按三条线分析：

**线路 A（讲解风格）**：
- 讲解方式：详细 vs 简洁，理论 vs 实践
- 比喻举例：喜欢用什么例子解释抽象概念
- 节奏控制：快慢、停顿、重点强调

**线路 B（教学特点）**：
- 提问方式：启发式提问 vs 直接提问
- 纠错方式：严厉指出 vs 委婉引导
- 鼓励方式：夸奖标准、批评语气

**线路 C（标志性元素）**：
- 口头禅：「这道题太简单了」「注意看黑板」
- 经典比喻：某个知识点的标志性讲解方式
- 特殊习惯：擦黑板方式、讲课姿势

### Step 4：确认并写入

向用户展示摘要，确认后写入文件到 `./teachers/{slug}/`。

---

## 进化模式

用户追加新材料时，分析增量内容并 merge 到对应部分。

用户纠正时说「他不会这样」「她应该是」，更新对应内容。

---
---

# Teacher.skill Creator (Claude Code Edition)

## Trigger Conditions

Activate when the user says:
- `/teacher`
- "Help me create a teacher skill"
- "I want to distill my teacher"
- "New teacher"

---

## Main Flow: Create a New Teacher Skill

### Step 1: Basic Info (3 questions)

1. **Name/Nickname** (required): What do you call them? e.g., "Teacher Li", "Mr. Zhang"
2. **Basic Info** (one sentence): Subject, age group, personality traits
   - Example: `High school math teacher, 40 years old, strict but fair, loves using real-life examples`
3. **Special Style** (optional): Their most iconic teaching style, catchphrase, or habit

### Step 2: Source Materials

```
How would you like to provide materials?

  [A] Classroom recordings/videos
      Record a segment explaining a concept

  [B] Lesson plans/presentations
      Preparation documents, PPT, exercise explanations

  [C] Exam papers/homework annotations
      Handwritten corrections, comments

  [D] Chat records
      WeChat/QQ messages with the teacher

  [E] Paste text
      Copy-paste directly
```

### Step 3: Analyze & Generate

Analyze collected materials along three tracks:

**Track A (Explanation Style)**:
- Explanation approach: detailed vs concise, theory vs practice
- Analogies: what examples used to explain abstract concepts
- Pacing: fast vs slow, pauses, emphasis on key points

**Track B (Teaching Traits)**:
- Questioning style: Socratic questions vs direct questions
- Correction style: stern vs gentle guidance
- Encouragement: praise standards, criticism tone

**Track C (Iconic Elements)**:
- Catchphrases: "This question is too easy", "Watch the blackboard"
- Classic analogies: Signature way of explaining a concept
- Special habits: How they erase the board, teaching posture

### Step 4: Confirm & Write

Show summary to user, write files to `./teachers/{slug}/` after confirmation.

---

## Evolution Mode

When user adds new materials, analyze delta and merge into relevant sections.

When user corrects with "they wouldn't do that" / "they should be", update content.
