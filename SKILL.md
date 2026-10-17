---
name: writing-academic
description: Use when writing, editing, reviewing, or translating into English any academic or technical text (paper, abstract, thesis, proposal, report, caption, rebuttal), or when unsure about English numbers, abbreviations, units, ranges, hyphens, italics, verb tense, voice, or wordy phrasing.
---

# Writing Academic English

## Overview

Follow the target venue's style guide first. Without one, use APA 7 for general academic writing and the IEEE Editorial Style Manual for engineering and computer science. Clarity rules come from the Federal Plain Language Guidelines. Details, examples, and sources are in `reference.md`.

**If this skill folder contains `personal-style.md`, read it before writing.** It holds the author's personal style, and its rules override this file when they differ.

## Rules most often broken

| Rule | Correct | Incorrect |
|---|---|---|
| Define every abbreviation at first use, separately in the abstract and in the body | You Only Look Once (YOLO), Common Objects in Context (COCO), comma-separated values (CSV) | fine-tuned on COCO with YOLOv8 (never defined) |
| Never guess an expansion; if the source does not give it, write [expansion?] and ask the author | PN-ACC [expansion?] | an invented expansion |
| After defining an abbreviation, use only the abbreviation | … mAP … mAP | alternating "mAP" and "mean average precision" |
| Spell out small numbers: APA zero–nine, IEEE one–ten | APA: nine images, 10 images. IEEE: ten images, 11 images | |
| Use numerals with units, percentages, statistics, and decimals | 5 mm, 95%, 0.25 | five mm, 95 %, 95 percent |
| Never start a sentence with a numeral | Five models were tested. A total of 2,000 images … | 5 models were tested. |
| English decimal point and thousands comma | 0.75, 2,000 | 0,75, 2.000 |
| Ranges: en dash, unit once; "from … to" in words | 10–20 cm, from 5 to 50 | 10 cm–20 cm, from 5–50 |
| "Data" is plural | The data were collected. | The data was collected. |
| No contractions | do not, cannot | don't, can't |
| Keep subject, verb, and object close | Faster R-CNN serves as the baseline. It is a two-stage detector … | Faster R-CNN, a two-stage detector trained on the same data, serves as the baseline. |
| Uncover hidden verbs | analyze, review, apply | perform an analysis of, carry out a review of, make an application |
| Cut wordy phrases | to, now, can, because, several | in order to, at this point in time, is able to, due to the fact that, a number of |
| One term per concept | test set … test set | test set … evaluation data … held-out split |
| No slash for "and/or" | X, Y, or both | X and/or Y |
| Hyphenate a compound modifier only before the noun | a two-stage detector; the detector has two stages | a two stage detector |
| Do not italicize technical terms; italicize only a key term at first use with its definition | point proposal, test set | *point proposal*, *test set* (Indonesian convention) |
| Verb tense by purpose | Past for methods and results ("The model achieved"); present for implications and conclusions ("The results indicate"); in a proposal, future or present for planned work ("The models will be compared") | shifting tense within a paragraph; past tense for work not yet done |
| One spelling system, American for IEEE | behavior, center, analyze | behaviour, centre in an IEEE paper |

## Workflow

1. Write the draft.
2. Check each sentence against the table, and against `personal-style.md` if present.
3. Read consecutive sentence pairs. Each sentence should follow from the one before it, without a repeated clause or a forced causal link.

## Failures seen in baseline tests

- YOLOv8, COCO, R-CNN, and CSV were never defined.
- "Faster R-CNN, a two-stage detector trained on the same data, serves as the baseline" split the subject from its verb.
- "Five models were tested, including a random forest model, which achieved …" left "which" ambiguous.
- When told to define every abbreviation, an agent invented an expansion for an abbreviation the source never expanded.
- Translating "Pengujian ini dilakukan dengan mengadaptasi APGCC" as "The test adapts APGCC" kept an Indonesian subject that cannot perform the English verb. Rebuild the sentence around a real agent: "The study does this by adapting APGCC".
