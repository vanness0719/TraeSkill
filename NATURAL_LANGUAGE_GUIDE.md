# Trae Natural Language Activation Guide

Trae can automatically identify and call the expert roles in `.trae/Skills` based on your **natural language intent**. You don't need to remember complex paths; just communicate as you would with a real team of experts.

---

## ⚡️ Core Activation Methods

### 1. Full-Process "One-Sentence" Start (Highly Recommended)
If you have a new idea, just say:
> **"I want to develop a [Project Name], please take me through the full process."**

**Trae's Reaction**:
- Automatically activates [universal-dev-team](.trae/Skills/universal-dev-team/SKILL.md).
- Plays the role of **Team Lead** to set the pace.
- Sequentially calls **PM -> Architect -> Developer -> QA** roles.

### 2. Intent-Driven Role Auto-Assignment
Trae listens for specific keywords to switch expert modes:

| When you mention... | Trae's Automatic Role |
| :--- | :--- |
| "Code is messy", "Architecture design", "Tech stack" | **01/02 Architect** |
| "UI looks bad", "Not professional", "Design audit" | **02 Designer** |
| "Flutter", "Mobile App" | **03 Flutter Expert** |
| "React", "Next.js", "Slow performance" | **03 React Performance Expert** |
| "Database slow", "SQL error" | **05 Database Expert** |
| "How to test", "Automation script" | **04 Testing Expert** |
| "Marketing copy", "Promote this" | **09 Operations Expert** |

---

## 💡 Tips to Make Trae Smarter

### 1. Be Explicit with "Identity" Expectations
While Trae auto-assigns, you can guide it more precisely:
- *"As a **Security Specialist**, check this login logic for vulnerabilities."*
- *"Use the **Flutter Expert** Clean Architecture pattern to write this code."*

### 2. Request "Skill Library Compliance"
Trae's Skills library stores many best practices. When asking it to write code, you can add:
- *"Please refer to your **Skills Library standards** for the implementation."*
- *"Optimize this list according to **Skill Module 03** performance requirements."*

**💡 Advanced Guides**: 
- **[Common Development Skills & Scenarios Guide](./DEVELOPER_SKILLS_GUIDE.md)**: Lists detailed skills and trigger words for each stage.

### 3. Feedback Loops in "Team" Mode
In `universal-dev-team` mode, Trae will pause after each stage. You can say:
- *"I approve the PM's requirements; please proceed to the **Architecture Design** stage."*
- *"The code is done; now please have the **QA Expert** write test cases."*

---

## 🛠 Maintain Your "Spells"
If you find Trae misinterprets an intent:
1. Open the corresponding `SKILL.md`.
2. Add your preferred expressions to the "How to Use" or "Trigger Words" section.
3. Trae will match based on your personal habits next time.
