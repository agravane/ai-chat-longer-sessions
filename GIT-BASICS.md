# Keep track of your work with git

Git is a free tool that saves a numbered checkpoint of a folder each time you ask.
You can see what changed, and go back to any checkpoint. It stays on your computer.
Nothing goes online unless you choose that later.

## The idea: one Dev folder

Keep every project as a folder inside one parent folder. We suggest:

- Mac / Linux: `~/Dev` (a folder named Dev in your home folder)
- Windows: `C:\Dev` or `Documents\Dev`

Example:

```
Dev/
  volunteer-emails/
  trip-planning/
  school-essays/
```

One project = one folder = one git history. Pick your own spot if you prefer; the point is one known place.

## Set it up once

1. Install git: https://git-scm.com/downloads (accept the defaults).
2. Make your Dev folder.
3. Ask your AI: "Set up git tracking for my Dev folder. Ask me where it is and how I want to track my work, then walk me through each step one at a time."
   (If you filled in the paste block, it will already ask.)

## Each project

Ask the AI: "Start tracking this project folder with git." It will give you two or three commands to paste into a terminal opened in that folder.

## The habit: save a checkpoint

When a job reaches a good state (a draft you like, a fixed bug, a finished list), say:
"Save a checkpoint called: <what changed>."
The AI gives you the commands; the plain words are `git add .` then `git commit -m "<what changed>"`.

Good moments to save: before you let the AI make a big change, and after you check it worked.

## Undo and look back

- "What changed since my last checkpoint?" (`git status`, `git diff`)
- "Show my last 10 checkpoints." (`git log --oneline -10`)
- "Put this file back the way it was at the last checkpoint." (`git restore <file>`)

Ask the AI to explain a command before you run it. If it is unsure, it should say so.

## Rules that keep you safe

- Checkpoints are local only. Uploading to GitHub or any website happens only when you ask for it by name.
- Never put passwords, card numbers, or API keys in tracked files. Keep them in a file named `.env` and ask the AI to add `.env` to `.gitignore` so git skips it.
- Do not use `--force` or delete history unless you understand it and say so.
- Back up your Dev folder (external drive or a cloud folder). Git on one laptop is a checkpoint, not a backup.
