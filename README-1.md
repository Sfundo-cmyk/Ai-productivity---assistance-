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

- **Frontend:** HTML5, CSS3, vanilla JavaScript
- **AI models:** OpenAI `gpt-4o-mini` or Google Gemini `gemini-1.5-flash`, chosen by the user
- **Storage:** the user's API key and provider choice are saved only in the browser's `localStorage` — never sent anywhere except directly to the chosen AI provider
- **Hosting:** deployable on GitHub Pages, Netlify, Vercel, or any static host

## Getting started

1. Open `index.html` in a browser (or deploy it to a static host — see below).
2. Click the status pill in the top right corner and add your own API key:
   - [OpenAI API keys](https://platform.openai.com/api-keys)
   - [Google AI Studio (Gemini) API keys](https://aistudio.google.com/app/apikey)
3. Pick a tool from the sidebar and use it.

No installation, dependencies, or server setup are required.

## Deploying

**GitHub Pages**
1. Push this repository to GitHub.
2. In the repository settings, enable GitHub Pages and point it at the `main` branch (root).
3. Your site will be live at `https://<username>.github.io/<repo-name>/`.

**Netlify**
1. Drag and drop the project folder into [Netlify Drop](https://app.netlify.com/drop), or connect the GitHub repository for continuous deployment.

## Prompt engineering approach

Each tool sends its own fixed system prompt rather than relying on one generic chat instruction, so the model's behaviour stays scoped and predictable:

- **Email:** *"You write concise, professional workplace emails. Include a subject line. Tone: {tone}."*
- **Meeting:** *"Summarize into: Summary, Decisions Made, Action Items (with owner if mentioned)."*
- **Tasks:** *"Break the goal into a short, ordered, numbered task list. One line per task."*
- **Research:** *"Answer concisely and factually. If unsure of a changeable fact, say so and recommend verifying it."*

## Responsible and ethical use

- **Key ownership:** users provide and control their own API key; Deskmate never collects, logs, or transmits it anywhere other than the chosen AI provider.
- **Human review built in:** every output is a draft. It is the user's responsibility to review a generated email, task list, summary, or research answer before sending, acting on, or relying on it.
- **Honest about limits:** the research assistant is prompted to flag uncertainty on facts that may have changed rather than stating them as certain.
- **No hidden data use:** there is no analytics, tracking, or server-side storage. All state lives in the user's own browser.

## Project context

Built as part of the CAPACITI AI Skill Accelerator Programme, demonstrating applied use of AI tools (OpenAI / Gemini APIs), prompt engineering, and responsible AI practice in a functional, deployable solution.

## License

For educational/portfolio use.
