# Learning Notes

[English](README.md) | [简体中文](README.zh-CN.md)

A Codex skill for notes that help you remember **how you learned**, not just what a textbook says.

It turns real conversations, exercises, screenshots, and practical work into notes from the learner's perspective. Questions, mistaken ideas, corrections, and unresolved difficulties remain visible. Related concepts follow a learning journey rather than becoming an ever-growing pile of files.

## The organizing idea

```text
What was I trying to solve?
        ↓
Where did I get stuck?
        ↓
What did I need to learn first?
        ↓
Which explanation or action changed my understanding?
        ↓
What can I do now, and what remains unresolved?
```

The narrative connects these steps. Topic notes provide depth only where needed. An index helps you find them again. A small clarification may need just one page.

## What the skill emphasizes

- **Real experiences:** verifiable words and actions, without invented emotions, progress, dates, or scores.
- **Personal recall:** recognizable questions and familiar examples, with first-person wording grounded in evidence.
- **Reviewable corrections:** retain the original task and key conditions, the learner's answer, the error and correction, and recorded follow-up practice. Mark original misconceptions in red with explicit labels; distinguish missing source material from supplementary examples.
- **Connected notes:** causal transitions, appropriate prerequisites, and one canonical home for each full explanation.
- **Useful diagrams:** clarify distinctions such as location versus content or inputs versus return values; label assumptions.
- **Honest learning status:** distinguish recognizing an answer, filling blanks, writing independently, and testing it yourself.
- **Appropriate filing:** prerequisites belong in foundations, linked from the main subject.

A request to edit the skill does not authorize rewriting your knowledge base.

## Choose a language

Both variants implement the same method and use the same skill name, `learning-notes`. **Install one variant, not both.** The variant selects the language of the instructions; it does not require notes to use that language. Specify your preferred output language when needed.

| Variant | Skill folder |
| --- | --- |
| Simplified Chinese | [skills/zh-CN/learning-notes](skills/zh-CN/learning-notes) |
| English | [skills/en/learning-notes](skills/en/learning-notes) |

Each folder contains its own `SKILL.md`, UI metadata, and supporting reference and can be installed independently. The English variant is a translation of the Chinese source, version 0.1.1.

## Install

Download or clone this repository:

```sh
git clone https://github.com/Lain006/learning-notes.git
```

Copy your chosen **whole** `learning-notes` folder, including `references` and `agents`, into the `skills` directory under your active Codex home:

- If `CODEX_HOME` is set: `$CODEX_HOME/skills/learning-notes`.
- Otherwise: `~/.codex/skills/learning-notes`.

For English instructions, copy `skills/en/learning-notes`. If a skill with that name already exists, compare or back it up before replacing it. Open a new Codex chat after installation. Automatic selection remains enabled by default; explicit invocation is also available.

## Use

```text
Use $learning-notes to organize this learning session into my notes.
Preserve my real questions, mistakes, corrections, and practical work.
Connect the topics through one coherent learning journey instead of
splitting everything into separate pages. Follow my knowledge base's structure.
```

For scattered notes:

```text
These notes are accurate but scattered. Use $learning-notes to connect
this set through a main narrative, keeping detailed explanations in one place.
```

For later sessions:

```text
Update my learning notes with this session. Preserve the earlier mistakes,
but distinguish what I can now do independently from what I can only follow.
```

Provide the conversation, exercise answers, screenshots, or existing notes you want organized. If no personal learning record is available, the skill should say so rather than manufacture one.

## Example: a journey instead of a topic list

An illustrative sequence might connect:

> Function forms → receiving a return value → variable names versus values → returning versus printing → running an example → memory locations → pointers.

The point is to explain **why each step became necessary**. This is a structural illustration, not a claim about any user's real history. Technical detail can live in linked topic notes; the narrative must still make sense without opening every link.

## Format and verification

Markdown knowledge bases and other note formats can be supported. Obsidian-specific features are optional, not dependencies. Check supported rendering, durable image paths, links, and readable red corrections. Plain labels accompany colors so meaning survives formats without HTML.

Both language packages pass the bundled skill-creator structural validator. Structure checks do not prove teaching quality or mastery. User practice, the organizer's automated checks, and unverified examples must remain distinct in generated notes. The translation has been reviewed for matching scope and constraints; it has not been independently evaluated across learning scenarios.

## Improve it through real use

Feedback is welcome on evidence fidelity, narrative continuity, filing, length, and navigation. Prefer narrow changes based on actual failures to accumulating mandatory sections. Update both language variants and their references together; do not silently rewrite users' existing notes.

This repository contains the reusable method and structural examples, not private conversations, personal notes, screenshots, machine-specific paths, or credentials.
