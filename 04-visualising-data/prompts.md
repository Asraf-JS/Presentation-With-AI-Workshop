# 04 — Visualising Data: Prompts

This page has two parts. Part 1 is tied to the Nusantara Capital before deck and walks you through the workshop exercise. Part 2 is a set of prompts you can take away and use on any deck after the workshop.

Use these in **ChatGPT, Copilot Chat, or any AI chat tool**.

---

## Part 1 — Workshop Exercise

Open the before deck before you start: [Download NC_Q3_2025_Before.pptx](../01-rethinking-presentations/NC_Q3_2025_Before.pptx)

### Step 1 — Fix slide 4 (Revenue Performance)

Slide 4 has a 7-segment pie chart showing revenue by business unit. Run this prompt to get a better approach.

```
I have a slide titled "Q3 Revenue Performance" showing revenue by business
unit using a pie chart with 7 segments. The values are:

Asset Management: 22%
Investment Banking: 18%
Treasury: 15%
Retail: 14%
Advisory: 13%
Insurance: 11%
Others: 7%
Total: RM 4.2M

Problems with the current chart:
- 7 segments make comparison impossible
- No clear point or headline
- The chart shows everything but says nothing

Tell me: (1) what chart type to use instead, (2) how to sort the data,
(3) which segments to highlight and why, and (4) write a new slide title
that states the point rather than labelling the data.
```

### Step 2 — Fix slide 8 (Budget Utilisation)

Slide 8 has a clustered bar chart comparing actual spend vs target across 8 categories. Every bar is labelled and the chart has a grey background.

```
I have a budget utilisation slide with a clustered bar chart. It shows
actual spend vs target for 8 categories:

Salaries: Actual 420K, Target 400K (OVER budget by 20K)
Consultancy: Actual 145K, Target 160K (under)
Travel: Actual 68K, Target 80K (under)
Technology: Actual 55K, Target 60K (under)
Training: Actual 38K, Target 40K (under)
Office: Actual 24K, Target 30K (under)
Marketing: Actual 18K, Target 20K (under)
Misc: Actual 12K, Target 10K (slightly over)

The current chart has every bar labelled, a grey background, and two
series which makes it cluttered.

The audience is senior leadership. The point I want to make is that
only one category is over budget and it is not a concern.

Recommend: (1) chart type, (2) what to remove from the current chart,
(3) what to highlight, (4) a new slide title.
```

### Step 3 — Fix slide 5 (Project Status table)

Slide 5 has a 10-row, 6-column table with 9pt font. Run this prompt to simplify it.

```
I have a project status slide with a table showing 10 projects across
6 columns: Project Name, Owner, Start Date, Planned End Date, Status,
Key Issues.

Status breakdown:
- 2 projects Delayed: Project Helang (vendor issues), Talent Dev Plan
  (HR sign-off pending)
- 1 project At Risk: Project Rimau (resource gap since resignation)
- 7 projects On Track

The audience is the CEO and two division heads. They have 2 minutes
for this slide. The decision they need to make is whether to approve
a headcount reallocation for Project Rimau.

Help me: (1) decide which rows to keep, (2) which columns to cut,
(3) how to highlight the at-risk items, (4) write a title that makes
the single point this slide needs to make.
```

### Step 4 — Rewrite all chart and table titles

After fixing the charts, run this prompt to check all your data slide titles at once.

```
Here are the current titles for all data slides in my quarterly review deck:

4. Q3 Revenue Performance
5. Project Status Update
6. Key Achievements
8. Budget Utilisation
9. Risks and Issues

For each title: (1) is it a label or a point? (2) rewrite it as an
assertive headline that states the insight, not the topic. Use the
Nusantara Capital context: revenue exceeded target, two projects at
risk, budget mostly on track with one exception.
```

### Step 5 — Generate a process diagram for the approval flow

The before deck has no visual showing how the headcount reallocation decision works. Use this Mermaid prompt to create one.

```
Write Mermaid flowchart code for this approval process:

1. Department Head identifies resource gap in Project Rimau
2. Department Head submits reallocation request to CEO
3. CEO reviews: if approved, one headcount moves from Project Angkasa
   to Project Rimau for 8 weeks
4. If not approved, Department Head escalates to Board
5. After 8 weeks, headcount returns to Project Angkasa

Use flowchart LR direction. Label each step clearly. Show the decision
point as a diamond shape.
```

Paste this into ChatGPT or Copilot Chat. Copy the Mermaid code it returns and render it at [mermaid.live](https://mermaid.live) to preview the diagram, then screenshot it for use in PowerPoint.

---

## Part 2 — Try It Yourself

### Chart selection prompt

Save this prompt and use it whenever you are not sure which chart to use:

```
You are a data visualisation advisor for corporate presentations.

I have a slide with this data: [describe your data or paste the numbers]

The audience is: [describe your audience]
The point I want to make is: [write your one-sentence insight]

Tell me:
1. What chart type to use and why
2. What chart type to avoid and why
3. What to label and what to remove
4. A suggested slide title that states the insight, not the topic
5. Whether my data needs any context to be meaningful (target,
   comparison, time period)

Keep your answer practical. One chart recommendation, not a list.
```

### Simplifying tables

```
I have a data table with [X] rows and [Y] columns. The audience is
[describe audience]. They have [X] minutes for this slide.

The point I want to make is: [your insight]

Help me: (1) identify which rows to keep, (2) which columns to cut,
(3) how to highlight the key data, (4) write a slide title that makes
the point.

Here is the table: [paste your table]
```

### Writing insight-driven chart titles

```
I have a [chart type] showing [describe the data]. The current title
is "[paste your title]". Here are the numbers: [paste key values].

Rewrite the title to make a point. Give me 3 alternatives with
different angles.
```

### Avoiding common chart mistakes

```
I have a [describe your chart]. The issues I can see are [describe
problems]. The key point I want to make is [your insight].

What should I replace it with and how should I redesign the slide?
```

---

## Mermaid Diagram Prompts

Use these in **ChatGPT or Copilot Chat** to generate diagrams you can paste into [mermaid.live](https://mermaid.live) and export as images.

### Process flow

```
Write Mermaid flowchart code for this process:
[describe your process in plain English, step by step]

Requirements:
- Direction: left to right (LR)
- Show decision points as diamond shapes
- Label each arrow clearly
- Keep node labels under 5 words each
```

### Project timeline

```
Write Mermaid Gantt chart code for this project plan:

Project: [name]
Start date: [date]

Tasks:
- [Task 1]: [start date] to [end date]
- [Task 2]: [start date] to [end date]
- [Task 3]: [start date] to [end date]

Mark [task name] as a milestone.
Show [task name] as critical path.
```

### Org chart or hierarchy

```
Write Mermaid flowchart code for this organisational structure:
[describe the hierarchy in plain English]

Use top-down direction (TD). Keep labels short.
```

### Sequence diagram

```
Write a Mermaid sequence diagram showing this interaction:
[describe who does what, in what order]

Participants: [list the people or systems involved]
```

---

## Napkin.ai Prompts

Go to [napkin.ai](https://napkin.ai) and paste any of these directly into the text input.

### Framework visual

```
[Paste your concept, process, or framework as bullet points or
plain sentences. Napkin will generate multiple visual interpretations
automatically. Pick the one that fits your slide, adjust the colours
to match your brand, and export as PNG.]
```

### Tips for better Napkin outputs:
- Use short, parallel phrases rather than full sentences
- Structure content as numbered steps or labelled categories
- If the output is too complex, reduce your text to 3 to 5 key points
- Use the "regenerate" option to get different layout styles

---

## Copilot Chat Visual Prompts

Use these at [copilot.microsoft.com](https://copilot.microsoft.com) (free).

### Ask for a diagram image

```
Create a simple diagram showing [describe your concept]. Style:
clean, corporate, minimal. Use navy blue and white. No background.
Suitable for a PowerPoint slide.
```

### Ask for Mermaid code

```
Write Mermaid code to visualise [describe your process or structure].
Then show me a preview description of what the diagram would look like.
```

### Ask for chart recommendation

```
I have this data: [paste your data]. I am presenting to [audience].
My key message is [one sentence]. What is the best chart type and
why? Give me one recommendation only.
```

---

*Back to: [Module 04 Notes](./README) | Next: [05 — Canva for Visual Design](../05-canva-design/)*
