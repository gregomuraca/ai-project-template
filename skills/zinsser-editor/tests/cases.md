# Behavioral Tests

These cases define expected behavior. They are not exact-output snapshots.

## 1. Corporate abstraction

**Input**

> In order to successfully leverage our innovative solution, organizations can utilize our seamless platform to drive meaningful business outcomes.

**Expected behavior**

Identify inflated phrasing, vague claims, duplicated verb concepts, and unsupported modifiers. Do not invent specific outcomes that are absent from the source.

## 2. Already good

**Input**

> I didn't know what the machine was doing, so I opened it.

**Expected behavior**

Leave unchanged unless surrounding context reveals a factual or tonal problem.

This is the core restraint test.

## 3. Technical accuracy

**Input**

A technically precise explanation containing domain terminology necessary for correctness.

**Expected behavior**

Clarify syntax and explain terms where useful, but keep necessary distinctions and terminology intact.

## 4. Personal voice

**Input**

A paragraph containing fragments, contractions, and dry humor.

**Expected behavior**

Do not normalize the fragments or contractions merely to make the prose more formal. Preserve comic timing.

## 5. Analyze mode

**Request**

> Tell me what is wrong with this draft, but don't rewrite it.

**Expected behavior**

Return diagnosis only. No replacement paragraphs.

## 6. Edit mode

**Request**

> Clean this up.

**Expected behavior**

Use minimal intervention. Do not restructure the argument unless necessary to fix a clear coherence problem.

## 7. Rewrite mode

**Request**

> Rewrite this as a concise executive memo. You can restructure it.

**Expected behavior**

Structural changes are allowed. Facts, uncertainty, and intended decisions remain intact.

## 8. Quotation preservation

**Input**

An interview excerpt with grammatically irregular but distinctive speech inside quotation marks.

**Expected behavior**

Do not silently rewrite the quotation.

## 9. Weak criticism

**Input**

> The interface is excellent and intuitive.

**Expected behavior**

Identify the unsupported judgment and request or use available criteria/evidence. Do not substitute different unsupported praise.

## 10. Generic conclusion

**Input**

A conclusion that only repeats the article and adds a vague optimistic future sentence.

**Expected behavior**

Recommend ending at the last substantive point or replacing the conclusion with an earned implication, not generic uplift.

## 11. Passive voice used well

**Input**

> Three samples were contaminated during transport.

Context does not identify the person responsible.

**Expected behavior**

Do not force active voice merely to satisfy a rule.

## 12. Meaning versus brevity

**Input**

A longer sentence whose qualifiers materially limit the claim.

**Expected behavior**

Preserve necessary qualifiers even when removing them would make the sentence shorter.
