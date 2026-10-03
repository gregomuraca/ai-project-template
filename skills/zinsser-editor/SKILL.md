---
name: zinsser-editor
description: Edit, rewrite, or audit nonfiction for clarity, simplicity, unity, structure, precision, voice, and rhythm using operational principles derived from William Zinsser's On Writing Well.
---

# Zinsser Editor

## Purpose

Improve nonfiction without replacing the writer.

Use this skill to make prose clearer, leaner, more precise, and better structured while preserving the author's meaning, voice, register, and factual integrity.

Do not imitate William Zinsser's personal style. Apply editorial principles, not stylistic mimicry.

## Modes

Choose the least destructive mode that satisfies the request.

### Analyze
Diagnose the writing. Do not rewrite unless the user asks.

### Edit
Default for requests such as "improve," "polish," "tighten," or "clean up." Make the smallest changes that materially improve the text.

### Rewrite
Use only when the user explicitly permits restructuring, substantial shortening/expansion, or a new format.

### Audit
Evaluate finished writing against the quality criteria below. Do not rewrite unless requested.

## Core editing order

Work in this order. Do not line-edit prose that may later be removed.

1. **Intent**
   - What is this piece trying to make the reader know, feel, decide, or do?
   - What is the central point?

2. **Unity**
   - Is the scope stable?
   - Are point of view, tense, tone, and stance coherent?
   - Does every section belong to the same piece?

3. **Structure**
   - Does the opening start the actual piece?
   - Does each paragraph create a reason to continue?
   - Is information ordered according to what the reader needs next?
   - Does the ending arrive naturally rather than announce itself?

4. **Clarity**
   - Prefer direct syntax.
   - Break unnecessary syntactic nesting.
   - Simplify the explanation without simplifying away necessary meaning.

5. **Clutter**
   - Remove redundant words, empty transitions, inflated phrases, needless qualifiers, jargon, and repeated conclusions.
   - Keep words that contribute meaning, rhythm, emphasis, humor, or voice.

6. **Precision**
   - Prefer specific nouns and strong verbs.
   - Replace vague abstractions only when the replacement is supported by the source material.
   - Preserve legitimate technical terminology.

7. **Voice**
   - Preserve characteristic vocabulary, cadence, contractions, humor, directness, formality, and degree of certainty.
   - Do not normalize distinctive human writing into generic professional prose.

8. **Sound**
   - Read for cadence, repetition, monotony, awkward rhythm, and punctuation.
   - Vary sentence length when the prose has become mechanically uniform.

9. **Restraint**
   - If a sentence is already clear, precise, natural, and appropriate, leave it alone.

## Non-negotiable rules

- Do not make a sentence more sophisticated merely to make it sound better.
- Do not invent facts, evidence, motives, emotion, lessons, outcomes, or certainty.
- Do not alter quotations unless the user explicitly asks to edit quoted material and doing so is appropriate.
- Do not replace precise technical distinctions with simpler but inaccurate language.
- Do not remove intentional ambiguity unless it harms the stated purpose.
- Do not add enthusiasm, hype, jokes, or emotional framing that is absent from the source.
- Do not assume shorter is always better.
- Do not convert every passive construction to active voice; change it only when agency or clarity improves.
- Do not apply grammar rules mechanically when natural contemporary usage is appropriate.

## Common failure patterns to detect

Treat these as diagnostic signals, not automatic deletions:

- generic openers;
- throat-clearing;
- repeated setup before the real point;
- inflated corporate language;
- vague nouns such as "solution," "value," "impact," or "outcomes" without specifics;
- unnecessary qualifiers and intensifiers;
- weak verb + adverb combinations;
- nominalizations hiding actors and actions;
- generic transitions;
- excessive signposting;
- repeated "not X, but Y" constructions;
- forced groups of three;
- domain clichés;
- generic motivational endings;
- uniform sentence length;
- polished but ownerless prose.

## Voice-preservation check

Before finalizing, compare the original and revision for:

- sentence length;
- formality;
- vocabulary;
- directness;
- humor;
- technical density;
- contractions;
- first-person use;
- certainty;
- rhythm.

A revision that is smoother but less recognizable is not necessarily better.

## Form adaptation

Adjust the editing strategy to the form:

- **Business:** recover actors, actions, ownership, decisions, and outcomes.
- **Technical/scientific:** protect correctness and terminology; explain rather than dilute.
- **Interview/profile:** preserve distinctive quotations and observed detail.
- **Memoir/personal:** favor specific memory and authentic voice over exhaustive chronology.
- **Travel/place:** prefer observed detail over stock description.
- **Criticism/review:** require claim → criterion → evidence → reasoning.
- **Humor:** preserve timing and incongruity; do not explain the joke.

For the deeper rationale, read `references/principles.md`.
For sentence and paragraph diagnostics, read `references/diagnostics.md` only when needed.

## Output contract

### Analyze
Return:
1. what the piece is trying to do;
2. the strongest element to preserve;
3. issues ranked by impact;
4. a recommended editing strategy.

Do not rewrite.

### Edit
Return the improved text. Preserve structure unless a local structural fix is necessary. Explain only consequential changes when useful.

### Rewrite
Return the rewritten text. If structure, emphasis, or argument changed materially, state what changed.

### Audit
Evaluate:
- intent;
- unity;
- clarity;
- structure;
- specificity;
- clutter;
- voice;
- rhythm;
- semantic/factual integrity.

Rank recommendations by impact. Do not turn the audit into an unsolicited rewrite.

## Final quality gate

Before completing an edit, ask:

1. Is the meaning clearer?
2. Is the prose more precise?
3. Is anything important lost?
4. Does this still sound like the writer?
5. Did I introduce generic AI phrasing?
6. Did I edit anything that was already working?

If meaning, voice, or accuracy degraded, revise again.
If a change is merely different rather than better, restore the original.
