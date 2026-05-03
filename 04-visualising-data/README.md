---
layout: default
title: 04 — Visualising Data for Storytelling
---

# 04 — Visualising Data for Storytelling

A chart that shows everything tells nothing. This module covers how to choose the right chart for the message you are trying to communicate, how to turn raw data tables into slides that say something, and how to use AI tools to generate diagrams and visuals without a design background.

> **Prompts to Try:** Open the [copy-paste prompt exercises](./prompts) for this module.
> [Download Chart Examples Deck](./Module04_Chart_Examples.pptx)

---

## Choosing the Right Chart

Chart choice is not about aesthetics. It is about what question the chart is answering.

| If you want to show | Use this | Avoid this |
|---------------------|----------|------------|
| Change over time | Line chart or column chart | Bar chart used for time series |
| Comparison between categories | Horizontal bar chart | Pie chart with more than 3 segments |
| Part of a whole | Stacked bar or single percentage callout | Pie chart with many slices |
| Compare to a target | Variance bar chart | Clustered bar with too many series |
| A single important number | Large text callout | Any chart |
| Project or process status | Simplified 3-row table | Full raw table from Excel |

### When to skip the chart entirely

Not all data needs a chart. If your single most important point is one number, "revenue was RM 4.2M against a target of RM 3.8M", the most powerful slide is a big number on a clean background with context underneath it. A chart here adds nothing and dilutes the impact.

---

## Common Chart Mistakes in Corporate Decks

**The pie chart with too many segments.** Human eyes cannot accurately compare pie slices when there are more than three. Use a horizontal bar chart instead — the differences are immediately readable.

**The 3D chart.** Three-dimensional effects distort actual values and make comparison harder. Use flat charts. Always.

**Two Y-axes.** Dual-axis charts look sophisticated but are almost always confusing. If you are combining two datasets with different scales, use two separate charts.

**Every data point labelled.** When every bar or point has a number attached, the chart becomes a table with decoration. Label only the values that matter: the highest, the lowest, the target, or the outlier.

**No baseline context.** "Sales increased 12%" compared to what? The same period last year? The target? Another region? Always give the number a reference point.

**Truncated Y-axis.** Starting a bar or line chart axis above zero artificially exaggerates differences. Unless there is a specific reason, start axes at zero.

---

## Turning Tables into Insights

Excel tables copied directly into PowerPoint are one of the most common problems in corporate decks. They are usually too small to read, contain more data than anyone needs, and make no point on their own.

### The three-step simplification process

**Step 1 — Identify the one thing you want the audience to know.**
Before you touch the table, answer: if this data could only say one thing, what is it? That answer becomes your slide title.

**Step 2 — Reduce the table to only what supports that point.**
If your point is "Project Rimau is behind schedule", you do not need every project's full status. Show only the relevant rows and columns.

**Step 3 — Highlight or annotate the key data.**
Use bold text or a colour highlight to draw the eye to the point you are making. The audience should not have to search for it.

---

## Data Storytelling Mistakes to Avoid

**Showing data without a point.** "Here is the data" is not a presentation, it is a document. Every data slide should make an assertion. The chart or table is the evidence.

**Burying the insight in the body text.** If the most important number is in bullet point 6 of 9, your audience will miss it. Lead with the insight.

**Using precision to signal credibility.** "Revenue was RM 4,218,437.62" is not more credible than "RM 4.2M", it is just harder to process. Round numbers are clearer and just as accurate for leadership presentations.

**Letting the data decide the story.** The data should support your argument, not generate it. Know what you want to say first, then find the data that proves it.

---

## AI-Generated Diagrams and Visuals

Charts are not the only visual tool available. For process flows, frameworks, org structures, and concept maps, AI can generate diagrams quickly without any design software. Three tools worth knowing:

### Mermaid Diagrams

Mermaid is a text-based diagram language. You write plain text instructions and it generates flowcharts, sequence diagrams, Gantt charts, and more. It works inside ChatGPT, GitHub, Notion, and several other tools.

**When to use it:** Process flows, decision trees, project timelines, system architecture, org charts.

**How it works:** You write a short code block describing the diagram, and the tool renders it as an image. You can then screenshot or export it for use in PowerPoint.

Example — a simple approval flow:

```
flowchart LR
    A[Submit Request] --> B{Manager Approval}
    B -- Approved --> C[Finance Review]
    B -- Rejected --> D[Revise and Resubmit]
    C -- Approved --> E[Execute]
    C -- Rejected --> D
```

This produces a left-to-right flowchart with decision branches. You can ask ChatGPT or Copilot Chat to generate Mermaid code for any process you describe in plain English.

**Mermaid diagram types available:**

| Type | Use for |
|------|---------|
| `flowchart` | Process flows, decision trees, approval workflows |
| `sequenceDiagram` | Step-by-step interactions between people or systems |
| `gantt` | Project timelines and milestones |
| `pie` | Simple part-of-whole (2 to 3 segments only) |
| `mindmap` | Brainstorming, concept mapping |
| `timeline` | Historical or project chronology |

### Napkin.ai

Napkin.ai converts plain text or bullet points into visual diagrams automatically. You paste your content and it generates multiple visual interpretations you can choose from, edit, and export.

**When to use it:** When you have a concept, process, or framework written out as text and want to turn it into a visual quickly without building it manually in PowerPoint or Canva.

**How it works:** Go to [napkin.ai](https://napkin.ai), paste your text, and it suggests several diagram styles. Pick the one that fits, adjust colours and labels, then export as PNG or SVG.

**Best for:** Frameworks (2x2 matrices, pyramids, cycle diagrams), process steps, comparison visuals, and concept illustrations for slide backgrounds.

### Copilot Chat Visuals

Copilot Chat (free web version at copilot.microsoft.com) can generate diagrams in several ways:

1. **Mermaid code** — ask Copilot to write Mermaid code for any process and render it using a Mermaid viewer
2. **Image generation** — ask Copilot to create a diagram or infographic illustration as an image (uses DALL-E under the hood)
3. **Table to visual** — describe a table and ask Copilot to suggest the best visual representation

**Limitation:** Copilot-generated images work well for conceptual illustrations but are less reliable for precise data charts. Use PowerPoint's built-in chart tools for anything with actual numbers.

---

*Back to: [03 — PowerPoint AI Features](../03-powerpoint-ai/) | Next: [05 — Canva for Visual Design](../05-canva-design/)*
