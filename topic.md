Ok, mình sẽ **viết lại full deck hoàn chỉnh từ đầu → cuối**, đã tối ưu:

- ✅ Storytelling rõ ràng
- ✅ Dev-centric (nghe là hiểu, dùng được ngay)
- ✅ Có flow: _Problem → Use → Trust → System → Scale_
- ❌ Không lan man tool / pricing

---

# 🎯 FULL SLIDE DECK (FINAL VERSION)

---

# 🟦 Slide 1 — Title

**AI in SDLC 2026: From Hype to Real Impact**

**Subtitle:**
How AI is actually used in real development workflows

---

# 🟦 Slide 2 — Objective

**What this session is about**

- Go beyond “AI hype”
- Focus on real developer workflows
- Show practical ways to use AI daily

---

**What you’ll gain**

- Apply AI across dev workflow
- Choose the right tools for each task
- Integrate AI into daily work

---

# 🟦 Slide 3 — Why Change Now?

**Reality today**

- Backlogs are growing
- Deadlines are shrinking
- Quality expectations are rising

---

**Pain points**

- Slow ticket understanding
- Time-consuming debugging
- Repetitive manual work

---

**Vision**

> AI removes repetitive work, not developers

---

# 🟦 Slide 4 — Before vs After AI

## Without AI

- Debug takes hours
- Manual test writing
- Slow code understanding
- Heavy reliance on senior devs

---

## With AI

- Faster debugging (trace + suggest fix)
- Auto-generated tests
- Instant code understanding
- AI-assisted review

---

### 💥 Key message

> AI accelerates every step of development

---

# 🟦 Slide 5 — Dev Workflow (Baseline)

## Debug

```
Receive → Understand → Reproduce → Trace → Fix → Verify
```

## Feature

```
Requirement → Design → Implement → Test → Iterate
```

## Non-code

- Script automation
- Analyze repo
- Write documentation

---

# 🟦 Slide 6 — Where AI Fits

| Step       | AI Support                 |
| ---------- | -------------------------- |
| Understand | Explain / đọc hiểu code    |
| Trace      | Tìm chỗ fix / analyze flow |
| Fix        | Suggest patch              |
| Test       | Generate unit test         |
| Review     | Review code                |
| Maintain   | Ghi comment                |
| Document   | Viết doc                   |

---

### 💥 Insight

> AI supports the entire lifecycle, not just coding

---

# 🟦 Slide 7 — Real Dev Use Cases

## 🧠 Code Understanding

- Explain codebase
- Summarize logic
- Understand unfamiliar systems

---

## 🔍 Debug & Fix

- Locate bug
- Trace data flow
- Suggest solution

---

## 🚀 Feature Development

- Generate boilerplate
- Implement feature
- Suggest architecture

---

## 🧪 Testing

- Generate unit test
- Cover edge cases

---

## 🔎 Code Review

- Detect issues
- Suggest improvements

---

## 📝 Documentation

- Write API docs
- Generate README
- Add comments

---

### 💥 Insight

> AI removes writing bottlenecks → Dev focuses on thinking

---

# 🟦 Slide 8 — ⚠️ Human-in-the-loop

**AI is not autonomous**

| AI       | Human    |
| -------- | -------- |
| Suggest  | Decide   |
| Generate | Review   |
| Analyze  | Validate |

---

### 💥 Key message

> Dev is no longer just coding
> → Dev becomes AI operator

---

# 🟦 Slide 9 — Levels of AI Usage

### 1. Assist

- AI suggests
- Dev decides

---

### 2. Copilot

- AI writes code
- Dev reviews

---

### 3. Autonomous (⚠️ Risk)

- AI loops itself
- Dev only approves

---

### 💥 Insight

> More autonomy = more risk
> → Human control is mandatory

---

# 🟦 Slide 10 — What is a Coding Agent?

**Agent ≠ Model**

- Model = generate text
- Agent = orchestrate workflow

---

### Architecture

```
Developer → Agent → Model Provider
```

---

### Examples

- Cursor
- Cline
- Claude Code

---

# 🟦 Slide 11 — Agent = Workflow Engine

AI does not run once
→ It runs a loop:

```
Read → Search → Analyze → Fix → Test → Retry
```

---

### 💥 Key idea

> AI is a multi-step reasoning system

---

# 🟦 Slide 12 — Example: Debug with Agent

```
1. Read code
2. Find related logic
3. Understand issue
4. Suggest fix
5. Generate patch
6. Run test
7. Analyze result
8. Retry if needed
```

---

### 💡 Reality

> One bug = multiple AI steps

---

# 🟦 Slide 13 — Usage Rule Count (CORE)

**Definition**

> 1 request = 1 reasoning step

---

### Not:

- ❌ 1 prompt = 1 request
- ❌ 1 task = 1 request

---

# 🟦 Slide 14 — Usage Breakdown

### Debug example

| Step    | Requests |
| ------- | -------- |
| Read    | 1        |
| Analyze | 1        |
| Fix     | 1        |
| Test    | 1        |
| Retry   | 1        |

---

👉 Total: **5–10 requests / task**

---

### 💥 Insight

> Cost comes from loops, not prompt size

---

# 🟦 Slide 15 — Why Usage Matters

- Estimate cost per task
- Detect infinite loops
- Optimize workflow
- Compare tools

---

### 💥 Key message

> If you don’t measure usage
> → you cannot scale AI

---

# 🟦 Slide 16 — Tool Selection Mindset

## ❌ Wrong way

- Choose trending tools
- Pick strongest model

---

## ✅ Right way

| Task          | Tool        |
| ------------- | ----------- |
| Quick ask     | Chat UI     |
| Codebase work | IDE agent   |
| Automation    | CLI agent   |
| Complex flow  | Multi-agent |

---

### 💥 Insight

> No best tool — only best fit

---

# 🟦 Slide 17 — Provider & Routing

**Why multiple models?**

- Different strengths
- Fallback
- Performance

---

### Architecture

```
Agent → Routing → Model Providers
```

---

### 💡 Dev takeaway

> Dev doesn’t manage models
> → Agent does

---

# 🟦 Slide 18 — AI Adoption Workflow

## Step 1 — Start small

- Debug
- Code explain

---

## Step 2 — Expand

- Test generation
- Code review
- Documentation

---

## Step 3 — Scale

- Agent workflows
- Automation loops

---

### 💥 Insight

> Start simple → then scale

---

# 🟦 Slide 19 — Where AI Fails

## Common issues

- Hallucination
- Wrong fixes
- Misunderstanding context
- Infinite loops

---

## Why?

- Poor context
- Weak prompt
- No human control

---

### 💥 Key message

> AI without control is unreliable

---

# 🟦 Slide 20 — Team Impact

With proper AI usage:

- Faster delivery
- Less repetitive work
- Better code quality
- More consistent output

---

### 💥 Insight

> AI scales team performance, not just individuals

---

# 🟦 Slide 21 — Developer Role is Changing

## Before

- Dev codes
- QA tests
- BA writes docs

---

## After (with AI)

1 Dev can:

- Code
- Test
- Review
- Document
- Debug

---

### 💥 Key message

> AI turns dev into full-cycle engineer

---

# 🟦 Slide 22 — Putting it all together

```
Dev Workflow
   ↓
AI Assist (Human-in-loop)
   ↓
Agent Loop
   ↓
Usage (Requests)
   ↓
Model Execution
```

---

# 🟦 Slide 23 — Key Takeaways

### 1. AI fits into dev workflow (not replace it)

### 2. Agent > Model

### 3. Usage Rule Count is critical

### 4. Human-in-the-loop is mandatory

---

# 🟦 Slide 24 — Closing

> AI will not replace developers
> Developers who use AI will replace those who don’t
