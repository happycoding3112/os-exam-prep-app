# 02159 Exam Trainer

A single-page study app for the DTU 02159 Operating Systems exam (10 December 2026: 20 short questions × 5 points, 4 hours).

## Features

- **Practice**: 99 questions across 11 topics in four kinds: *What prints?* (C snippets), *Find & fix*, *Work it out* (paging, page replacement, scheduling, deadlock safety) and *Explain*. Write your answer, reveal the model answer, rate yourself. New and missed questions come up more often.
- **Mock exam**: a random mix with a timer (20 questions / 4 h, 10 / 2 h or 5 / 1 h), then mark each answer 0–5 against the model answers.
- **Progress**: mastery per topic, mock exam history and a list of missed questions to drill.
- **Study plan**: a day-by-day plan from 19 November to the exam, with checkboxes.
- **Notes**: key points per topic and how answers are marked.

## Run it

It's one static file with no build step and no dependencies. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

Progress is stored in your browser's `localStorage`. When the page runs as a Claude artifact, it also syncs progress to your Claude account and offers optional "Grade with Claude" feedback; those features are hidden elsewhere.

## Notes

The questions and model answers are written from the course's example code and standard textbook topics (Tanenbaum & Bos, *Modern Operating Systems*). Check anything doubtful against the lecture slides. The OS Challenge questions are generic; compare them with your own group's specification.
