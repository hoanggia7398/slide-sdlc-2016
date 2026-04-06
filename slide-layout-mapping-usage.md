Here is the detailed documentation of the layout patterns from your Marp file, along with use cases and mapping rules. This is designed so your AI Agent can understand "If-Then" logic (If it encounters a specific type of information -> Choose the corresponding layout).

---

## 📖 How to Use Mapping Keys

### Reading Mapping Keys

Each layout is assigned a unique **mapping key** in the following format:
- In slide file: `<!-- LAYOUT-X: Layout Name -->` (placed immediately after `---` slide separator)
- In mapping file: `### <!-- LAYOUT-X --> Layout Name`

### Mapping Rules

| Mapping Key | Content Type | Corresponding Layout |
|-------------|--------------|----------------------|
| `LAYOUT-1` | Main title, project intro, new chapter | Title/Cover Slide |
| `LAYOUT-2` | Short list (3-4 items), core principles | 2-Column Focus Text |
| `LAYOUT-3` | Process, pipeline, step 1→2→3 | Split Flow Diagram |
| `LAYOUT-4` | Comparison, Before/After, Pros/Cons | Highlight Comparison |
| `LAYOUT-5` | 3 features, 3 pillars, 3 concepts | 3-Column Feature Cards |
| `LAYOUT-6` | Numbers, KPIs, %, metrics | Big Metrics/Stat Cards |
| `LAYOUT-7` | Quote, closing statement, takeaway | Big Quote/Statement |

### AI Agent Workflow

```
1. Analyze input content
2. Identify content type (trigger)
3. Look up corresponding mapping key
4. Apply layout from example-slide-style.md
5. Fill content following mapping guidelines
```

### Mapping Example

**Input:** "Software development process: Requirements → Design → Development → Testing → Deployment"

**Analysis:** Content is sequential with multiple steps → `LAYOUT-3`

**Result:** Use Split Flow Diagram with node-boxes containing: Requirements, Design, Development, Testing, Deployment

---

### <!-- LAYOUT-1 --> Title / Cover Slide (Intro / Section Break)
* **UI/UX Description:** Minimalist, focusing heavily on typography. It includes an "eyebrow" (small, uppercase, wide-spaced text) for context, and a massive Header (`h1`) using gradient text on a dark background. Faded navigation hint text sits at the bottom.
* **Suitable Use Cases:**
  * Introducing the main topic of the presentation.
  * Acting as section breaks (chapter titles) in a long deck.
* **Agent Mapping Guidelines:**
  * **Trigger:** When the input is a [Main Topic], [Project Name], or a signal starting a new section (e.g., "Part 1: Overview").
  * **Mapping:** `eyebrow` = Context/Category; `h1` = Topic Title (auto-insert `<br/>` to break lines if it exceeds 4 words).

### <!-- LAYOUT-2 --> 2-Column Focus Text (Core Principles)
* **UI/UX Description:** No boxes or cards, just large typography (32px). Bullet points use a custom blue arrow icon (`→`). The layout is split into 2 columns (`grid-template-columns: 1fr 1fr`) to keep the reading distance short and comfortable for the eye.
* **Suitable Use Cases:**
  * Core philosophies, principles, or visions.
  * A concise list of core values (3-4 items, very short, without descriptive paragraphs).
* **Agent Mapping Guidelines:**
  * **Trigger:** Input is a list of 3-4 items, each under 6 words, WITHOUT detailed explanations attached.
  * **Mapping:** Insert directly into the `<li>` tags within the `.points` block.

### <!-- LAYOUT-3 --> Split Flow Diagram (Processes & Pipelines)
* **UI/UX Description:** Screen is split in a `1 : 1.2` ratio. The left side contains a subtitle and explanatory text (bullet points). The right side features a series of geometric blocks (nodes) connected by arrows, creating a linear flow with a hover-glow effect.
* **Suitable Use Cases:**
  * Step-by-step processes.
  * Product lifecycles.
  * Linear data flows or system architectures (Pipelines).
* **Agent Mapping Guidelines:**
  * **Trigger:** Input describes a chronological or sequential order (e.g., "First... then...", "Step 1, Step 2, Step 3").
  * **Mapping:** Put the detailed summary into the bulleted list on the left. Extract extremely short "Action Keywords" (1-2 words) to place inside the `.node-box` elements on the right.

### <!-- LAYOUT-4 --> Highlight Comparison (Before vs. After)
* **UI/UX Description:** Two glassmorphism cards placed side-by-side. The visual trick here is that one card is highlighted (`.card.highlight`) with a brighter border and text (Primary Blue), subconsciously directing the viewer's attention to that specific card.
* **Suitable Use Cases:**
  * Before / After scenarios.
  * Old Solution vs. New Solution (Traditional vs. Modern).
  * Pros / Cons comparisons.
* **Agent Mapping Guidelines:**
  * **Trigger:** Input contains contrasting ideas, or keywords like "However," "Instead of... we use...", "Versus".
  * **Mapping:** Assign "Old/Weak/Past" states to the standard card. Assign "New/Better/Future" states to the `.card.highlight`.

### <!-- LAYOUT-5 --> 3-Column Feature Cards (Pillars & Details)
* **UI/UX Description:** An equal 3-column grid (`grid-3`). Each column holds a card containing a small Heading and a short paragraph (2-3 lines). This mimics the standard "Features" section found on SaaS landing pages.
* **Suitable Use Cases:**
  * Product features or capabilities.
  * 3-pillar action plans or strategies.
  * Detailed explanations for 3 specific concepts.
* **Agent Mapping Guidelines:**
  * **Trigger:** Input is a list of exactly 3 items (or the AI can synthesize the info into 3 core pillars), where each requires both a Title and a Description.
  * **Mapping:** `h2` = Keyword/Feature Name; `<p>` = Short description (strictly keep under 150 characters to prevent breaking the layout).

### <!-- LAYOUT-6 --> Big Metrics / Stat Cards (KPIs & Impact)
* **UI/UX Description:** Also uses a 3-column grid, but instead of long text, it focuses entirely on massive numbers (72px, gradient text) and a very short label below them. Highly visual and "glanceable."
* **Suitable Use Cases:**
  * Reporting results, KPIs, and metrics.
  * Showcasing growth (%, x-times).
  * Quantitative milestones (e.g., Cost reduced, time saved, active users).
* **Agent Mapping Guidelines:**
  * **Trigger:** Input contains distinct quantitative data points (numbers, %, currency symbols) meant to highlight achievements or results.
  * **Mapping:** Extract the core number/metric for `.stat-num` and summarize the context for `.stat-label` (maximum 3-4 words).

### <!-- LAYOUT-7 --> Big Quote / Statement (Takeaways)
* **UI/UX Description:** Centered on the screen, bypassing default headers. Features huge text with prominent quotation marks as a visual anchor. Below it is the author/source in uppercase, widely-spaced font (`letter-spacing`).
* **Suitable Use Cases:**
  * Direct quotes from experts, executives, or customer feedback.
  * A strong closing statement or Key Takeaway that reinforces the main message.
  * A "breathing room" slide placed between heavy data/chart sections.
* **Agent Mapping Guidelines:**
  * **Trigger:** Input is a complete, impactful sentence, a strong assertion, or explicitly attributed to a specific person/organization.
  * **Mapping:** Core content goes into `.quote-text`; Source/Author goes into `.quote-author`.

---

**System Prompt Suggestion for your AI Agent:**
> *"You are an Expert Presentation Designer AI. Your task is to analyze raw input text and automatically map it to 1 of 7 predefined Marp UI layouts. If the content contains a step-by-step sequence, use Layout 3 (Split Flow). If it contains KPI numbers highlighting achievements, use Layout 6 (Big Metrics). You must automatically summarize, split, and format the text to strictly fit the character limits and node constraints of your chosen layout."*