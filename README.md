

## Mizan-AI

Mizan-AI is an evaluation-oriented dataset designed to test how well Large Language Models (LLMs) handle Hassaniya Arabic, a low-resource Arabic variety spoken mainly in Mauritania and surrounding regions.

The project focuses on capability assessment, not fine-tuning. It provides carefully designed prompts to probe understanding, generation, and linguistic competence in Hassaniya across multiple modalities.

⸻

## Motivation

Most LLM benchmarks focus on high-resource languages or standardized dialects (MSA, English, French). Hassaniya is largely absent from evaluation datasets, which leads to:
	•	Overestimated multilingual performance
	•	Silent failure modes in African and Maghrebi dialects
	•	No visibility into reasoning vs memorization behavior

Mizan-AI exists to expose those gaps.

⸻

## Scope

This repository contains prompt-based evaluation datasets, not model outputs.

The goal is to measure:
	•	Comprehension
	•	Generation quality
	•	Dialect awareness
	•	Code-switching behavior
	•	Robustness to non-standard orthography

⸻

## Dataset Structure

The dataset is organized into three core folders, each representing a distinct capability axis:

Mizan-AI/
│
├── understanding/
│   ├── comprehension.json
│   ├── paraphrasing.json
│   └── intent_detection.json
│
├── generation/
│   ├── storytelling.json
│   ├── translation.json
│   └── explanation.json
│
├── speech/
│   ├── phonetic_prompts.json
│   ├── oral_style_generation.json
│   └── transcription_reasoning.json
│
└── metadata/
    └── schema.md

1. understanding/
Prompts that test whether a model actually understands Hassaniya input:
	•	Meaning extraction
	•	Paraphrasing
	•	Implicit intent
	•	Cultural references

2. generation/
Prompts that require producing Hassaniya:
	•	Natural responses
	•	Narratives
	•	Explanations
	•	Controlled transformations (register, tone, length)

3. speech/
Textual proxies for spoken language:
	•	Phonetic spellings
	•	Oral syntax
	•	Speech-like ambiguity
	•	ASR-style reasoning tasks

⸻

## Prompt Design Principles
	•	Multiple valid answers when appropriate
	•	No forced standardization (orthography varies on purpose)
	•	Dialect-first, not MSA-derived
	•	Designed for evaluation, not demo quality

⸻

## What This Is Not
	•	Not a translation dataset
	•	Not a training corpus
	•	Not standardized Arabic
	•	Not optimized for leaderboard gaming

⸻

## Intended Use
	•	LLM benchmarking
	•	Dialect robustness analysis
	•	Research on low-resource language evaluation
	•	Comparative model studies (open vs proprietary)

⸻

## Contribution

all contribution is welcome

