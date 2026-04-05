# EduConnect — MediBot

AI chatbot built with Microsoft Copilot Studio for a fictional Romanian private tutoring platform.

## What it does

MediBot helps parents and students:
- Find information about available subjects and tutors
- Check pricing and packages
- Book tutoring sessions (fully automated flow)
- Get matched with the right tutor based on subject, level, and availability

All conversations are in Romanian.

## Context

EduConnect is a fictional company I created as a portfolio project. It offers private tutoring (meditații) for students preparing for Evaluarea Națională (8th grade) and Bacalaureat (12th grade) in Romania.

## Tech used

- Microsoft Copilot Studio
- Knowledge base (custom .txt files for subjects, tutors, pricing, FAQ)
- System topic customization (greeting, fallback, escalation — all in Romanian)

## Repo structure

```
educonnect-medibot/
├── README.md
├── TESTING.md
├── screenshots/
├── knowledge-base/
│   ├── general.txt
│   ├── subjects-tutors.txt
│   ├── pricing.txt
│   └── faq.txt
└── config/
    └── MediBot_CopilotStudio_Config.md
```

## Testing

See [TESTING.md](TESTING.md) for all test cases, expected vs actual results, and screenshots.

## What I learned

- Designing conversation flows and fallback logic
- Writing a knowledge base that an AI agent can actually use well
- Tuning system topics and trigger phrases for a non-English language
- Thinking about UX from the parent's and student's perspective
