# Deskmate — AI-Powered Workplace Assistant

Deskmate is a browser-based AI assistant built for the CAPACITI AI Skill Accelerator Programme. It automates five common workplace tasks — email drafting, meeting summarizing, task planning, quick research, and general chat — using an AI model of the user's choice (OpenAI or Google Gemini).

## Live demo

[Add your deployed URL here once published]

## Features

| Tool | What it does |
|---|---|
| **Email generator** | Turns a short description into a ready-to-send, professionally toned email |
| **Meeting summarizer** | Condenses raw notes or a transcript into a summary, decisions made, and action items |
| **Task planner** | Breaks a stated goal into an ordered, practical checklist |
| **Research assistant** | Answers work questions concisely and flags anything that may need verifying |
| **Chatbot** | General-purpose conversational help for quick workplace questions |

## How it works

Deskmate is a single static HTML file — no backend, no build step, no framework. It calls the AI provider's API directly from the browser using an API key that the user provides and controls.

## Getting started

1. Open `index.html` in a browser (or deploy it to a static host).
2. Click the status pill in the top right corner and add your own API key.
3. Pick a tool from the sidebar and use it.

## Responsible and ethical use

- Users provide and control their own API key; it's never collected or logged by Deskmate.
- Every output is a draft — review before sending, acting on, or relying on it.
- No analytics, tracking, or server-side storage.

## Project context

Built as part of the CAPACITI AI Skill Accelerator Programme.
