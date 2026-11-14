---
name: learning-notes
description: "Turn real learning conversations, exercises, and practical records into learner-centered notes. Preserve questions, misconceptions, corrections, and verification evidence, connecting topics through a coherent learning journey. Use for personal learning notes, reflection, and incremental updates; do not turn ordinary textbook summaries into invented personal experiences."
metadata:
  version: "0.1.1"
---

# My Learning Journey Notes

Create notes that help their owner recall why they were confused, how their understanding changed, and what they actually did. Ground the notes in real experiences, write from the learner's perspective, connect them through a coherent narrative, and judge them by how effectively they support recall. Keep them accurate and familiar; do not replace the learning journey with an encyclopedic summary.

## 1. Establish evidence and where the material belongs

- Use the current conversation, the user's answers and screenshots, and directly relevant existing notes. Read the destination knowledge base's rules, index, and related entries before choosing a location. Do not search unrelated private history to manufacture a richer story.
- Distinguish four sources: the user's words or actions, course or reference material, the organizer's explanations, and unverified inferences. Use quotation marks only for verifiable quotations. Label paraphrases as summaries rather than presenting them as exact words.
- Preserve meaningful questions, answers, edits, runs, abandoned attempts, and consciously deferred topics. Do not invent emotions, motives, progress, scores, dates, or personal conclusions such as "I finally understood."
- When evidence is incomplete, organize what is supported and mark missing records where relevant. Ask only about consequential gaps. Distinguish event dates from the date of compilation; do not rewrite a conversation spanning several days as one day's events.
- Classify material by its knowledge dependencies, not just the course being watched. For example, C syntax learned before data structures belongs in an accessible prerequisite section, with connections from the main course. Reuse existing entries rather than automatically creating another top-level subject.

## 2. Connect the journey before deciding how many notes to create

Before drafting, answer briefly: What was I trying to solve? Why did I get stuck? What did I need to learn first? Which example or action changed my understanding? What can I do now, and what remains unresolved? These answers form the learning narrative.

Keep two orders distinct: describe experiences in their actual order or clearly identified phases; explain concepts in the order of their prerequisites. Never change the history to make the story smoother.

- Start with one narrative note that can be read from beginning to end. Split off a topic only when it has independent review value, reuses an existing entry, or materially improves readability.
- Give each full explanation, detailed correction, and example one canonical home. Elsewhere, use a short contextual sentence and a precise link, not copied paragraphs. Brief summaries of experiences may remain in the narrative.
- An index helps readers navigate; the narrative explains why the learner arrived here; topic notes provide depth. A short task may combine these roles in one note. Do not mandate all three, or a fixed number such as eight notes.
- Make transitions explicit: for example, "To receive a function's result, I first needed to distinguish a variable's name from its value; to understand pointers, I then separated values from locations." A list of links is not a narrative.
- At a topic's entrance, explain which question in the journey it resolves. At its exit, explain what it makes possible next and link to genuinely relevant material. Branches may return to the narrative; do not force all knowledge into a single straight line.
- Keep the main text focused on experiences that changed understanding. Put environment details, long code, original exercises, and supplementary limits in topic notes, collapsible sections, or attachments as needed. Do not present everything at equal prominence.

For multiple notes, fragmented existing content, or examples of correction context, read [references/coherent-structure.md](references/coherent-structure.md).

## 3. Preserve changes in understanding from the learner's perspective

Start from an evidenced "At the time, I thought..." and connect it to the specific question and correction. Familiarity comes from recognizable words, examples the learner used, and genuine uncertainty, not slogans, dramatic monologues, or generic encouragement.

A meaningful turning point often includes: the original idea → the precise error or gap → the explanation, comparison, or action that helped → the corrected understanding → evidence of ability and remaining uncertainty. Adapt to the material rather than mechanically filling five fields every time.

- Describe the specific confusion rather than blaming "weak foundations," such as mixing up a pointer's own address with the address it stores.
- Never leave an uncorrected misconception standing alone in the main text. Mark it in red, label it "Original misconception" or "Original answer," and place the correction immediately after it. Color must not be the only signal.
- In Obsidian, `<span style="color:#ff6b6b;">Original misconception: ...</span>` is an option; check readability in the active theme. If the destination does not support HTML, use its native red text or error callout instead of exposing raw tags to readers.
- Label partially or conditionally correct reasoning as "Needs refinement" rather than marking everything wrong. Do not attribute a mistake to the user if they never made it.
- For each detailed correction, retain enough of the original exercise or task to attempt it again: the given conditions, requirements, and code, inputs, or diagram information needed to understand the mistake. Match the user's answer to that task, then explain the error, the correction, and any recorded follow-up practice. An isolated mistake quotation and a one-line correction are insufficient. Retain meaningful original scores with their basis; do not invent grading. Brief experience summaries may provide essential context and a precise link to this full record.
- To fill gaps, first check available original records directly related to this learning session. Explicitly mark exercises or steps that cannot be recovered. Label newly written explanatory examples as "Organizer's supplementary example" rather than presenting them as original exercises or user experiences. Preserve the sequence of scaffolded answers, independent attempts without hints, and later questions. Do not upgrade one correct fill-in answer to independent mastery or impose fixed fields on every passage.
- Support claims such as not yet studied, can follow an explanation, can recognize, can complete a scaffold, can write independently, and verified by running with matching evidence. Separate the organizer's automated runs from the user's own practice. Do not force a proficiency rating without evidence.
- Clearly label deliberately deferred difficulties, for example, "Use this established form for now; revisit the reason later." Do not append a harder lecture just to appear comprehensive.

## 4. Use familiar scenarios and diagrams to make abstractions concrete

- Prefer the same problem scenario already used by the learner or teacher. Change one requirement or concept at a time. Do not switch scenarios when doing so adds cognitive load.
- Make each diagram answer a specific confusion: location versus content, input versus return, changing a variable versus changing its target, or what changes between steps. Label variables, values, addresses, arrows, and necessary assumptions; attractive boxes alone are insufficient.
- For state changes, keep the layout consistent before and after, identifying what changes and what remains unchanged. State the limits of analogies; do not imply nonexistent memory layouts or physical proportions.
- Choose a format the destination can actually render. Use text diagrams for simple relationships and supported diagrams or local images for more involved ones. Store images in the knowledge base's durable attachment directory and embed them, rather than referencing only temporary files.
- Put a short conclusion beside each figure. Tables and checklists may aid lookup, but should not repeat the entire explanation. Omit visuals that do not reduce the effort of understanding.

## 5. Check structure and facts before delivery

Do not assess completeness alone; check whether the narrative can be followed:

1. Can a reader quickly identify the starting point, main turning points, and current state? Is it clear why each major section appears where it does?
2. Can the learner find a topic using the question they remember asking? Does every new topic have an entrance and a way back?
3. Are full explanations or code repeated, branches excessive, or sections present only to satisfy a template? Consolidate repetition and link to the canonical explanation.
4. Without opening the original chat, can a reader use the detailed correction and its explicitly linked material to tell what the task was, how I answered, what went wrong, why the correction works, and what was subsequently verified? Are mistakes clearly marked and corrected nearby? Are unresolved or deferred topics honestly retained? Are technical explanations and analogies accurate?
5. Do links, heading anchors, image paths, and rendering work? When possible, inspect the actual reading view, especially red text, code, tables, and diagrams. Do not install plugins or change global appearance merely to check layout.
6. Verify complete code, calculations, or testable claims proportionately. Label intentionally incorrect examples and fragments that cannot run alone. State the boundary between automated checks and the learner's own work.

Finish with a concise entry link, filing location, meaningful verification, and remaining gaps. Respect existing naming conventions. Do not automatically create MEMORY.md or treat note organization as permission to write global memories.

## 6. Improve this skill through real use

When feedback arrives, identify whether the problem concerns evidence, narrative, classification, length, or navigation. In an authorized skill-editing task, adjust the relevant rule or example precisely. Do not silently rewrite other notes or accumulate universal requirements for every individual case.

When changing structure, check both the entrypoint and its references, keeping each rule in one consistent place. Use relevant new cases to assess coherence without sacrificing truthfulness. Do not claim to have solved all fragmentation without comparing actual outcomes.
