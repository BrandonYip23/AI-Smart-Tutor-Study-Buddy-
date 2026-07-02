[README.md](https://github.com/user-attachments/files/29610423/README.md)
# 🎓 AI Tutor — A Custom Claude Skill

A multi-subject AI tutor built as a Claude Skill, designed for exam prep and homework help. It adapts difficulty and teaching style to each learner in real time, so every session feels personalized instead of generic.

## Why This Exists

Most AI "tutoring" is really just answer-generation — ask a question, get a solution, learn nothing. This skill is built to do the opposite: it meets students where they are, adjusts pacing and difficulty on the fly, and pushes them to actually understand the material rather than just finish the assignment.

## ✨ Features

- **Multi-Subject Coverage** — Works across math, science, language arts, history, and other core subjects without needing a separate skill per topic.
- **Adaptive Difficulty** — Continuously reads how a student is performing and adjusts question difficulty, pacing, and scaffolding accordingly. Struggling learners get more support; confident learners get pushed further.
- **Personalization** — Remembers a student's strengths, weak spots, and preferred explanation style within a session (and across sessions, if memory is enabled) to tailor future explanations.
- **Exam Prep Mode** — Structured practice sessions that simulate test conditions, target weak areas, and track readiness over time.
- **Homework Help Mode** — Guides students through problems step-by-step instead of just handing over answers, reinforcing understanding along the way.

## 🚀 Getting Started

### Prerequisites

- Access to Claude (claude.ai, Claude Code, or the Claude API) with Skills support enabled.

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/BrandonYip23/AI-Smart-Tutor-Study-Buddy.git
   ```
2. Copy the skill folder into your Skills directory:
   ```bash
   cp -r ai-tutor-skill /path/to/your/skills/
   ```
3. Enable the skill in your Claude environment (see your platform's Skills documentation for details).

### Usage

Once enabled, just start a conversation and describe what you need help with:

```
"Help me prep for my algebra exam next week — I struggle with quadratic equations."
"Can you walk me through this chemistry homework problem?"
"Quiz me on World War I causes, medium difficulty."
```

The skill will assess the student's current level from context (or a quick diagnostic), then adapt questions, hints, and explanations as the session progresses.

## 🧠 How Adaptive Difficulty Works

1. **Baseline check** — A few warm-up questions or diagnostic prompts establish a starting difficulty level.
2. **Live adjustment** — Correct answers nudge difficulty up; repeated mistakes trigger simpler explanations, worked examples, or a step back to foundational concepts.
3. **Style matching** — The skill notices whether a student responds better to visual analogies, step-by-step logic, or real-world examples, and leans into what works.
4. **Progress tracking** — Session summaries highlight what was mastered and what needs more practice, so future sessions pick up where the last one left off.

## 📁 Repository Structure

```
.
├── ai-tutor-skill/
│   ├── SKILL.md          # Core skill definition and instructions
│   ├── prompts/          # Prompt templates for different modes
│   └── examples/         # Example sessions and use cases
└── README.md
```

## 🛠️ Customization

Want to tailor the tutor further? You can:
- Edit `SKILL.md` to change tone, subject emphasis, or teaching philosophy.
- Add subject-specific prompt templates under `prompts/`.
- Adjust difficulty-scaling logic to match your grading scale or curriculum standards.

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request with improvements, new subject templates, or bug fixes.

## 📄 License

[Add your license here — e.g., MIT]

---

Built for students who want to actually *learn*, not just get answers.
