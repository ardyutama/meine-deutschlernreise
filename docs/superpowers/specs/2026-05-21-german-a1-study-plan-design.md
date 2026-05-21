# Design: Meine Deutschlernreise — A1 Study Plan

**Date:** 2026-05-21  
**Status:** Approved  
**Approach:** Immersion-First with Multiple Streams (coding-interview-university style)

---

## Overview

A structured, checkbox-tracked German A1 study plan inspired by [coding-interview-university](https://github.com/jwasham/coding-interview-university). The plan uses Netzwerk Neu A1 as the textbook backbone, supplemented with curated free resources across multiple learning streams.

### Learner Profile

- **Starting level:** Absolute zero
- **Daily commitment:** 1-2 hours
- **Timeline:** 4-6 months (24 weeks)
- **Textbook:** Netzwerk Neu A1 (full package: Kursbuch, Arbeitsbuch, Intensivtrainer, online exercises, videos)
- **Motivation:** All-round (career, travel, culture, personal growth)
- **Constraint:** Free resources only (beyond already-owned textbook)

---

## Project Structure

```
meine-deutschlernreise/
├── README.md                        # Main study plan with checkboxes
├── AGENTS.md                        # Template for generating A2, B1, etc.
├── resources/
│   ├── free-a1-resources-guide.md   # Detailed resource descriptions
│   └── visual-fun-content-a1.md     # YouTube, shows, comics, games
├── docs/
│   └── superpowers/specs/           # Design documents
├── a1/
│   ├── 00-getting-started.md        # Setup, tools, mindset
│   ├── 01-week-01-02.md             # Alphabet, sounds, first words
│   ├── 02-week-03-04.md             # Greetings, introductions, numbers
│   ├── 03-week-05-06.md             # Family, friends, present tense
│   ├── 04-week-07-08.md             # Daily life, time, separable verbs
│   ├── 05-week-09-10.md             # Food, shopping, accusative case
│   ├── 06-week-11-12.md             # Review & Plattform 1-2
│   ├── 07-week-13-14.md             # City, directions, dative case
│   ├── 08-week-15-16.md             # Appointments, modal verbs
│   ├── 09-week-17-18.md             # Work, professions, prepositions
│   ├── 10-week-19-20.md             # Health, body, imperative
│   ├── 11-week-21-22.md             # Home, moving, Perfekt
│   └── 12-week-23-24.md             # Full review & exam prep
└── .agents/
    └── skills/
```

---

## README.md Design

### Structure

The README serves as the master study plan. It follows the coding-interview-university format:

1. **Header** — Title, description, motivation, how to use (fork + check boxes)
2. **Prerequisites & Setup** — Tools to install, accounts to create, mindset tips
3. **The Daily Routine** — 1-hour and 2-hour schedule templates
4. **Study Streams Explained** — What each stream is and why

5. **A1.1 — Foundations (Weeks 1-12, Netzwerk Kap 1-6)**
   - Week 1-2: Alphabet, Sounds & First Words
   - Week 3-4: Greetings, Introductions & Numbers
   - Week 5-6: Family, Friends & Present Tense
   - Week 7-8: Daily Life, Time & Separable Verbs
   - Week 9-10: Food, Shopping & Accusative Case
   - Week 11-12: Review & Plattform 1-2

6. **A1.2 — Building (Weeks 13-24, Netzwerk Kap 7-12)**
   - Week 13-14: City, Directions & Dative Case
   - Week 15-16: Appointments, Schedules & Modal Verbs
   - Week 17-18: Work, Professions & Prepositions
   - Week 19-20: Health, Body & Imperative
   - Week 21-22: Home, Moving & Perfekt
   - Week 23-24: Full Review & Exam Prep

7. **Fun & Immersion Resources** — YouTube, podcasts, shows, music, comics, games
8. **Tools & Daily Practice** — Anki setup, grammar refs, exam prep
9. **Key Principles** — Consistency > intensity, comprehensible input, active recall

### Weekly Block Format

Each 2-week block contains checkboxes grouped by stream:

```markdown
## Week 1-2: Alphabet, Sounds & First Words

**Netzwerk Neu:** Kapitel 1 — Guten Tag!  
**Theme:** Meeting people, German sounds, basic greetings  
**Grammar:** Personal pronouns, verb "sein", W-Fragen

### Core Textbook
- [ ] Read Kursbuch Kapitel 1 (dialogue + vocabulary)
- [ ] Complete Kursbuch exercises
- [ ] Complete Arbeitsbuch Kapitel 1
- [ ] Listen to all audio tracks for Kapitel 1

### Listening Stream
- [ ] DW ABC Course: Lessons 1-3 (alphabet & sounds)
- [ ] Nico's Weg: Episodes 1-3 (Meeting people)
- [ ] Coffee Break German: Episodes 1-5

### Vocabulary & Memory
- [ ] Set up Anki + download "German A1 Core Vocabulary" deck
- [ ] Add Kapitel 1 vocabulary to Anki (with articles!)
- [ ] Daily Anki reviews (15 min/day, every day)
- [ ] DW Deutschtrainer: Lessons 1-5

### Grammar Drill
- [ ] Lingolia: Personal pronouns + exercise
- [ ] Schubert-Verlag: Kapitel 1, Exercises 1-3

### Fun & Immersion
- [ ] Watch 1 episode of "Extra auf Deutsch" (just enjoy, don't stress)
- [ ] Learn German with Anja: "German Alphabet" video
- [ ] Label 10 objects in your home with German sticky notes

### Weekly Self-Check
> After this block, I can:
> - [ ] Say my name, where I'm from, and greet someone
> - [ ] Spell my name using the German alphabet
> - [ ] Recognize all German sounds including ä, ö, ü, ß
> - [ ] Count to 20
```

---

## AGENTS.md Design

The AGENTS.md serves as a reusable template for generating study plans at other levels.

### Contents

```markdown
# German Learning Plan Generator — Agent Instructions

## Purpose
Generate a structured, checkbox-tracked study plan for any CEFR level
using the same methodology as the A1 plan in this repository.

## Input Variables
- {{LEVEL}} — Target CEFR level (A2, B1, B2, C1, C2)
- {{TEXTBOOK}} — Primary textbook for that level
- {{DURATION_WEEKS}} — Expected timeline in weeks
- {{HOURS_PER_DAY}} — Daily time commitment

## Resource Categories (all must be included)
1. Core Textbook — chapter-by-chapter structural spine
2. Video Course — story-based, free (DW or equivalent)
3. Podcast Stream — level-appropriate audio input
4. Grammar Drills — online exercises matching textbook progression
5. SRS/Vocabulary — Anki decks or equivalent
6. Fun/Immersion — YouTube, shows, music, comics, games
7. Exam Prep — Goethe exam practice materials for that level

## Resource Evaluation Criteria
- FREE (or meaningful free tier)
- Level-appropriate (not too easy, not too hard)
- Targets a specific skill
- Has clear "how to use" instructions
- Community-endorsed (Reddit r/German, language forums, Goethe recommendations)

## Skill Balance by Level
| Level | Listening | Vocab | Grammar | Reading | Output |
|-------|-----------|-------|---------|---------|--------|
| A1    | 30%       | 25%   | 20%     | 15%     | 10%    |
| A2    | 25%       | 15%   | 20%     | 20%     | 20%    |
| B1    | 25%       | 10%   | 15%     | 25%     | 25%    |
| B2    | 20%       | 10%   | 10%     | 25%     | 35%    |
| C1    | 20%       | 5%    | 5%      | 30%     | 40%    |

## Weekly Block Template
[Include the exact markdown format used in the A1 README]

## Generation Process
1. Research free resources appropriate for {{LEVEL}} using 3-5 web searches
2. Map the textbook chapters to 2-week blocks
3. Find matching free resources for each block's theme
4. Select fun/immersion content at the right difficulty
5. Write weekly self-checks based on CEFR can-do statements
6. Include exam prep in final 4 weeks
7. Output in the same format as README.md

## Textbook Recommendations by Level
- A1: Netzwerk Neu A1 (12 chapters)
- A2: Netzwerk Neu A2 (12 chapters)
- B1: Netzwerk Neu B1 (12 chapters)
- B2: Aspekte Neu B2 or Sicher! B2
- C1: Aspekte Neu C1 or Erkundungen C1
```

---

## Curated Resources (A1 Final Selection)

### Core Resources (daily use)

| Resource | Type | Skill | URL |
|----------|------|-------|-----|
| Netzwerk Neu A1 | Textbook | All | (owned) |
| DW Nico's Weg A1 | Video course | Listening, Grammar | https://learngerman.dw.com/en/nicos-weg/c-36519789 |
| Coffee Break German S1 | Podcast | Listening, Grammar | https://coffeebreaklanguages.com/coffeebreakgerman/ |
| Anki | SRS app | Vocabulary | https://apps.ankiweb.net/ |
| Schubert-Verlag A1 | Exercises | Grammar, Listening | https://www.schubert-verlag.de/aufgaben/uebungen_a1/a1_uebungen_index.htm |

### Supplementary Resources (weekly use)

| Resource | Type | Skill | URL |
|----------|------|-------|-----|
| Lingolia German | Grammar ref | Grammar | https://deutsch.lingolia.com/en/grammar |
| DW Deutschtrainer | Vocab trainer | Vocabulary | https://learngerman.dw.com/en/deutschtrainer/c-56705009 |
| DW Harry gefangen in der Zeit | Audio drama | Listening | https://learngerman.dw.com/en/harry-gefangen-in-der-zeit-a1/c-55727738 |
| DW ABC Course | Pronunciation | Listening, Speaking | https://learngerman.dw.com/en/abc/c-39621991 |
| Learn German with Anja | YouTube | Grammar, Pronunciation | https://youtube.com/@LearnGermanwithAnja |

### Fun & Immersion Resources (keeps motivation high)

| Resource | Type | Skill | URL/Notes |
|----------|------|-------|-----------|
| Extra auf Deutsch | TV sitcom | Listening | Search "Extra auf Deutsch" on YouTube |
| Easy German (Super Easy) | YouTube | Listening, Culture | https://youtube.com/@easygerman |
| Goethe Stadt der Wörter | Game | Vocabulary | https://www.goethe.de/en/spr/kup/tsd.html |
| Sendung mit der Maus | Kids show | Listening | https://www.wdrmaus.de/ |
| German music | Songs | Listening, Vocab | Curated list in resources/ |

### Exam Preparation (Weeks 20-24)

| Resource | Type | URL |
|----------|------|-----|
| Goethe A1 Practice Exam | Full model exam | https://bfu.goethe.de/a1_sd1/ |
| DW Start Deutsch 1 Practice | Exam practice | https://learngerman.dw.com/en/start-deutsch-1/c-70467758 |
| DW Placement Test | Self-assessment | https://learngerman.dw.com/en/placementDashboard |

---

## Study Schedule Design

### Daily Routine (flexible between 1-2 hours)

**1-Hour Day:**
| Block | Duration | Activity |
|-------|----------|----------|
| Warm-up | 15 min | Anki reviews |
| Core | 20 min | Netzwerk Neu (textbook) |
| Input | 15 min | Podcast or Nico's Weg |
| Output | 10 min | Write/speak sentences |

**2-Hour Day:**
| Block | Duration | Activity |
|-------|----------|----------|
| Warm-up | 20 min | Anki reviews + new cards |
| Core | 30 min | Netzwerk Neu (textbook + exercises) |
| Drill | 15 min | Schubert/Lingolia grammar exercises |
| Input | 20 min | Podcast + Nico's Weg |
| Output | 20 min | Write 5 sentences, shadow audio |
| Cool-down | 15 min | Fun resource (YouTube, show, game) |

### Weekly Rhythm

| Day | Focus | Notes |
|-----|-------|-------|
| Monday | New chapter intro | Fresh textbook content + Anki cards |
| Tuesday | Grammar deep-dive | Textbook grammar + Lingolia |
| Wednesday | Workbook practice | Arbeitsbuch + Nico's Weg |
| Thursday | Listening day | Podcast focus + DW Deutschtrainer |
| Friday | Review + drill | Schubert exercises + chapter review |
| Saturday | Light/fun | Anki only + Extra auf Deutsch or music |
| Sunday | Output day | Write short text + record yourself speaking |

---

## Key Design Decisions

1. **Netzwerk Neu as backbone, not cage** — The textbook provides structure and grammar progression, but it's supplemented with 4+ other streams to prevent boredom and cover all skills.

2. **Checkbox tracking** — Every task is a checkbox. Fork the repo, mark progress with `[x]`. Visual progress is motivating.

3. **"I can now..." self-checks** — Each block ends with CEFR-aligned can-do statements so you know you're on track without needing external validation.

4. **Fun is mandatory, not optional** — Every week has a "fun" resource. This prevents burnout and builds positive associations with German.

5. **Anki is non-negotiable** — The one daily habit that must never be skipped, even on rest days. Spaced repetition is the highest-leverage activity for vocabulary.

6. **Free-only constraint respected** — Every resource in the plan is either free or has a meaningful free tier. The only paid item is the Netzwerk Neu textbook already owned.

7. **AGENTS.md enables scaling** — The template allows generating A2/B1/B2 plans with the same quality and structure, making this a long-term learning system.

---

## Success Criteria

After completing this plan (24 weeks), the learner should be able to:

- Pass the Goethe-Zertifikat A1 (Start Deutsch 1) exam
- Introduce themselves and ask basic personal questions
- Understand slow, clear speech about familiar topics
- Read simple texts (signs, menus, short messages)
- Write short notes and fill out forms
- Know ~800-1000 German words with correct articles
- Use present tense, basic cases (Nominative, Accusative, intro Dative), and common modal verbs

---

*Design approved: 2026-05-21*
