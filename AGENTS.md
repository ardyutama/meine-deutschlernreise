# German Learning Plan Generator — Agent Instructions

> Use this file to generate a structured study plan for any CEFR level (A2, B1, B2, C1, C2)
> following the same methodology as the A1 plan in this repository.

---

## Purpose

Generate a checkbox-tracked, multi-stream German study plan for a given CEFR level. The output should match the format and quality of the A1 `a1/README.md` in this repository.

---

## Input Variables

| Variable | Description | Example |
|----------|-------------|---------|
| `{{LEVEL}}` | Target CEFR level | A2, B1, B2, C1, C2 |
| `{{LEVEL_FOLDER}}` | Folder for this level | a2, b1, b2, c1, c2 |
| `{{TEXTBOOK}}` | Primary textbook for this level | Netzwerk Neu A2 |
| `{{DURATION_WEEKS}}` | Total timeline in weeks | 24 |
| `{{HOURS_PER_DAY}}` | Daily time commitment | 1-2 |
| `{{PREVIOUS_LEVEL}}` | What the learner has completed | A1 |

---

## Resource Categories

Every generated plan MUST include all 7 categories:

### 1. Core Textbook
- Chapter-by-chapter structural spine
- Specific Kursbuch + Arbeitsbuch tasks per week
- Plattform/review sections included

### 2. Video Course (free, story-based)
- DW Nico's Weg (A1, A2) or equivalent for higher levels
- Must be free and narrative-driven
- Include specific episode numbers mapped to textbook chapters

### 3. Podcast Stream
- Level-appropriate audio input
- Must start from the right difficulty (not too easy)
- Include episode numbers and pacing (e.g., "2 episodes/week")

### 4. Grammar Drills
- Online exercises matching textbook grammar progression
- Schubert-Verlag, Lingolia, or equivalent
- Link specific exercises to specific grammar topics

### 5. SRS / Vocabulary
- Anki deck recommendations
- New card targets per day
- Vocabulary milestones per block

### 6. Fun & Immersion
- YouTube channels appropriate for the level
- TV shows, films, music
- Games, comics, interactive content
- Must be genuinely enjoyable, not disguised homework

### 7. Exam Preparation
- Goethe exam format for that level
- Free practice materials
- Included in final 4 weeks of the plan

---

## Resource Evaluation Criteria

Before including any resource, verify:

| Criterion | Requirement |
|-----------|-------------|
| **Cost** | FREE or meaningful free tier (no paywalls for core content) |
| **Level** | Appropriate for {{LEVEL}} (not too easy, not too hard) |
| **Skill target** | Must clearly serve one or more skills |
| **Actionable** | Has a clear "how to use" instruction |
| **Quality** | Community-endorsed (Reddit r/German, forums, Goethe) or from reputable source (DW, Goethe, universities) |
| **Available** | Currently accessible (not dead links) |

---

## Skill Balance by Level

Adjust the daily time allocation based on level:

| Level | Listening | Vocabulary | Grammar | Reading | Output (Speaking+Writing) |
|-------|-----------|-----------|---------|---------|---------------------------|
| A1 | 30% | 25% | 20% | 15% | 10% |
| A2 | 25% | 15% | 20% | 20% | 20% |
| B1 | 25% | 10% | 15% | 25% | 25% |
| B2 | 20% | 10% | 10% | 25% | 35% |
| C1 | 20% | 5% | 5% | 30% | 40% |
| C2 | 15% | 5% | 5% | 30% | 45% |

**Key shift:** As level increases, output (speaking and writing) becomes dominant. Input (listening/reading) stays important but shifts to authentic materials.

---

## Weekly Block Template

Each 2-week block follows this exact structure:

```markdown
### Week X-Y: [Theme Title]

**{{TEXTBOOK}}:** Kapitel N — [Chapter Name]  
**Theme:** [2-3 word topic description]  
**Grammar:** [Key grammar points introduced]

#### Core Textbook
- [ ] [Specific textbook tasks]

#### Listening Stream
- [ ] [Specific episodes/resources with numbers]

#### Vocabulary & Memory
- [ ] [Anki tasks + vocabulary themes]

#### Grammar Drill
- [ ] [Specific exercises with URLs]

#### Fun & Immersion
- [ ] [Enjoyable activities related to the theme]

#### Weekly Self-Check
> After this block, I can:
> - [ ] [CEFR can-do statement 1]
> - [ ] [CEFR can-do statement 2]
> - [ ] [CEFR can-do statement 3]
```

---

## Generation Process

When generating a plan for a new level, follow these steps:

### Step 1: Research
- Search for free resources appropriate for {{LEVEL}}
- Check Reddit r/German wiki, DW offerings, Goethe materials
- Verify all links are active
- Find level-appropriate podcasts, YouTube channels, shows

### Step 2: Map Textbook
- Get the chapter list for {{TEXTBOOK}}
- Determine topics and grammar points per chapter
- Pace at 2 weeks per chapter (adjust if textbook has fewer/more chapters)
- Identify Plattform/review sections

### Step 3: Align Resources
- Match DW/equivalent video course episodes to textbook topics
- Find podcast episodes that cover similar themes
- Select Schubert-Verlag or equivalent exercises per grammar topic
- Choose fun content that matches each block's theme

### Step 4: Write Self-Checks
- Use official CEFR can-do statements for {{LEVEL}}
- Break them into specific, measurable checkboxes
- Align with what was taught in that block

### Step 5: Include Exam Prep
- Research Goethe exam for {{LEVEL}} (format, duration, sections)
- Find free practice exams online
- Place exam prep in the final 4 weeks

### Step 6: Output
- Write the main plan to `{{LEVEL_FOLDER}}/README.md`
- Store level-specific research and guides under `{{LEVEL_FOLDER}}/resources/`
- Store level-specific specs and notes under `{{LEVEL_FOLDER}}/docs/`
- Use the same markdown format as `a1/README.md`
- Include all sections: header, setup, daily routine, streams, weekly blocks, resources, principles
- Add level-specific tips and mindset notes

---

## Textbook Recommendations by Level

| Level | Primary Textbook | Chapters | Alternative |
|-------|-----------------|----------|-------------|
| A1 | Netzwerk Neu A1 | 12 | Menschen A1 |
| A2 | Netzwerk Neu A2 | 12 | Menschen A2 |
| B1 | Netzwerk Neu B1 | 12 | Menschen B1 |
| B2 | Aspekte Neu B2 | 10 | Sicher! B2 |
| C1 | Aspekte Neu C1 | 10 | Erkundungen C1 |
| C2 | Erkundungen C2 | 8 | (authentic materials primarily) |

---

## DW Course Availability

| Level | DW Course | Episodes |
|-------|-----------|----------|
| A1 | Nico's Weg A1 | 18 chapters |
| A2 | Nico's Weg A2 | 18 chapters |
| B1 | Nico's Weg B1 | 18 chapters |
| B2+ | No DW narrative course | Use authentic media |

---

## Level-Specific Notes

### A2 Notes
- Learner already has ~1000 words and basic grammar
- Focus shifts to past tense (Perfekt/Präteritum) and more complex sentences
- Add: Nebensätze (subordinate clauses with weil, dass, wenn)
- Podcast upgrade: Easy German Podcast becomes accessible
- Show upgrade: Easy German full episodes (not just Super Easy)

### B1 Notes
- Intermediate plateau is real — keep motivation high with engaging content
- Major grammar: Konjunktiv II, Passiv, relative clauses
- Start reading: simple German books (Kurzgeschichten, graded readers)
- Speaking practice becomes critical — consider Tandem partners
- Podcast: Slow German becomes appropriate at this level

### B2 Notes
- Transition to authentic materials (newspapers, podcasts for natives)
- Grammar refinement rather than new concepts
- Writing becomes important: longer texts, formal letters, arguments
- Consider: Deutsche Welle news, Tagesschau, ZEIT articles

### C1-C2 Notes
- Primarily authentic material consumption
- Focus on nuance, idioms, register, academic/professional German
- Writing: essays, reports, complex argumentation
- Speaking: discussions, presentations, debate
- Textbook plays a smaller role; authentic content drives learning

---

## Quality Checklist for Generated Plans

Before finalizing any generated plan, verify:

- [ ] All 7 resource categories are present
- [ ] The level lives in its own folder with `README.md`, `resources/`, and `docs/`
- [ ] All links are to free resources (or clearly marked free tier)
- [ ] Weekly blocks have specific, actionable checkboxes (not vague instructions)
- [ ] Self-checks use measurable can-do statements
- [ ] Fun resources are genuinely fun (not just more textbook work)
- [ ] Exam prep is included in final weeks
- [ ] Daily routine templates are realistic for the stated hours/day
- [ ] Grammar progression matches the textbook order
- [ ] Vocabulary targets are stated (e.g., "you should have ~1500 words by week 12")
- [ ] Transition to next level is mentioned at the end

---

*This template was created as part of the Meine Deutschlernreise project, May 2026.*
