---
name: blog-style-workflow
description: 'Generate blogs in a specific style, tone, language, and format from raw notes, transcripts, or source documents. Use when you need consistent brand voice, multilingual output, and publish-ready structure with quality checks.'
argument-hint: 'Provide topic, source content, target audience, desired tone/style, language, and output format.'
user-invocable: true
---

# Blog Style Workflow

## What This Skill Produces
- A publish-ready blog draft tailored to a requested style, tone, language, and audience.
- A quality pass that checks consistency, factual grounding, readability, and formatting.
- Optional variants (short, long, executive, technical) based on the same source.

## When to Use
- You have source material (transcript, notes, interview, docs) and need a polished blog.
- You need strict control over writing voice, language, or localization.
- You need repeatable quality checks before publication.

## Inputs
- Topic and purpose.
- Source material or links.
- Audience persona.
- Style constraints: voice, tone, sentence density, reading level, banned phrases.
- Language and locale (for example: English-US, English-UK, Spanish-LATAM).
- Output constraints: word count, section structure, CTA style, metadata requirements.

## Default Configuration
- Workflow mode: full multi-step workflow.
- Default language: English (US) when not specified.
- Style enforcement: fixed house style by default.
- Verification appendix: always include.

## House Style (Default)
- Voice: executive-neutral, clear, evidence-led, and practical.
- Tone: confident without hype, concise, and outcomes-oriented.
- Structure: short intro, clear H2 sections, actionable close.
- Language rules: active voice preferred, avoid jargon where plain words work.
- Banned patterns: exaggerated claims, unverifiable superlatives, vague impact statements.

## Decision Logic
1. If source quality is low (noisy transcript, fragmented notes):
   - Normalize and summarize source first.
   - Mark uncertain facts and request confirmation.
2. If style guidance is explicit (brand guide or samples):
   - Mimic structure and rhetorical patterns.
   - Enforce vocabulary and phrase constraints.
3. If style guidance is missing:
   - Enforce the fixed default house style defined in this skill.
4. If localization is requested:
   - Adapt idioms, spelling, and examples to locale.
   - Keep meaning fidelity over literal translation.
5. If compliance or sensitivity risk exists:
   - Redact sensitive details.
   - Add a verification note for claims requiring approval.

## Procedure
1. Capture brief
- Confirm topic, audience, format, language, and success criteria.

2. Ingest and clean source
- Remove transcription noise, filler, duplicated fragments, and obvious artifacts.
- Preserve named entities, dates, metrics, and key claims.

3. Extract story backbone
- Build outline: context, challenge, approach, outcomes, lessons.
- Sort points by signal strength and audience relevance.

4. Apply style and tone controls
- Calibrate voice (authoritative, conversational, technical, inspirational).
- Adjust pacing (short punchy vs long analytical paragraphs).
- Enforce banned words and preferred terminology.

5. Draft blog
- Produce headline options and one selected title.
- Write body with clear section headers and transitions.
- Include concrete examples, evidence, and actionable takeaways.

6. Run quality checks
- Factuality: every key claim tied to source material.
- Consistency: tone and terminology stable throughout.
- Readability: target level met, unnecessary jargon removed.
- Format: length, heading structure, and CTA meet requirements.

7. Produce final package
- Final draft.
- Alternate title options.
- Claim verification appendix (always required).

## Completion Criteria
- Blog matches requested style, tone, and language.
- No unsupported claims in final text.
- Formatting aligns with publishing constraints.
- Output is editable with minimal post-processing.

## Output Format
Return in this order:
1. Brief Confirmation
- Audience, tone, language, format, and word count target.

2. Blog Draft
- Title
- Optional subtitle
- Body with section headings
- CTA or closing

3. Quality Report
- Style adherence check
- Factuality notes
- Readability notes
- Open questions or approval-needed items

## Suggested Pairing
- Use with the Customer Zero Transcript Blogger agent when source content comes from SharePoint or Microsoft 365 transcripts and requires redaction-aware publication drafting.
