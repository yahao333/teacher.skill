---
name: teacher
description: "Distill a teacher's explanation style, teaching methods, and educational wisdom into an AI Skill. | 蒸馏老师的教学风格、讲解方法和教育智慧到一个 AI Skill 中。"
argument-hint: "[teacher-name-or-slug]"
version: "1.0.0"
user-invocable: true
allowed-tools: Read, Write, Edit, Bash
---

# teacher.skill 创建器

## 触发条件

- `/teacher`
- "帮我创建一个老师 skill"
- "我想蒸馏老师"

## 主流程

### Step 1：基础信息

1. **老师姓名/称呼**（必填）
2. **基本信息**：教什么科目、年龄段、性格特点
3. **教学风格**：严厉/温和、喜欢用什么方式讲课

### Step 2：原材料

- 课堂录音/视频
- 教案/课件
- 试卷/作业批注
- 聊天记录
- 直接粘贴

### Step 3：分析生成

- 讲解风格分析
- 处理问题方式
- 鼓励/批评方式
- 口头禅/金句

### Step 4：确认写入

---

# Teacher.skill Creator

## Trigger

- `/teacher`
- "Help me create a teacher skill"

## Main Flow

1. Basic info collection
2. Source materials import
3. Analyze teaching style
4. Confirm and write files
