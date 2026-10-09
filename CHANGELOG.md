# What's new in Sinag

Sinag shows the newest section before it updates (Settings → **What's new**) and once after.

## 0.9.8

### New
- **High Seas theme.** A pirate adventure from edge to edge: a real 16th-century sea chart full of
  ships and sea monsters behind everything, a dotted route to a red X, wanted-poster cards in
  parchment and ink, pirate-red buttons that press into the page, woodtype titles and pirate icons
  (ship, ship's wheel, spyglass, bottle, log book, map, treasure chest, compass, anchor).
- **Grimoire theme.** A world of spellbooks: a real medieval grimoire page behind everything inside
  a gold magic circle, every card an open vellum page with gold-leaf corners, glowing clover-green
  spell buttons, an anti-magic Stop, blackletter titles and spellbook icons.
- **Your own wallpaper.** Put any image from your PC behind Sinag and dim it to taste. It stays on
  your PC.
- **Glass.** Frosted panels over the theme or your wallpaper. Choose Follow Windows, On or Off in
  Settings → General.
  The two themes and the wallpaper come with a subscription.

### Fixed
- A wallpaper now always shows, whatever theme is on and however small the window.

## 0.9.7

### New
- **Learn: step-by-step learning paths.** Press the Learn button in the title bar (or
  Ctrl+Shift+L) and Sinag switches to a view made for learning. Name a topic, say React, pick your
  level and, if you like, a goal: the PM plans a path from the first install to something real,
  and you watch it appear module by module and step by step while it is written.
- **Every step teaches.** Each one has the idea in plain words, where it lives in a real project,
  a small task and questions to check yourself. Mark steps done and your progress is kept; add a
  new path any time.
- **Practise in a real project.** Give a path its own practice project, then on any step ask the
  tester to **check your work** like a mentor (it never rewrites it for you), or **let the team
  build it** and explain what you can learn from it. Nothing is sent until you press Send.
  Learn comes with a subscription.

### Improved
- **More skills for the team:** a lean, careful way of working (investigate first, small
  surgical fixes, safe refactors, reversible migrations, verify and stop), terse handoffs and
  reviews, browser automation, and more design references.

## 0.9.6

### Fixed
- **The team's engineering skills are back.** 0.9.5 left out the skills the PM and the developer
  use on every task (planning in small testable steps, software architecture and QA hardening).
  They ship with Sinag again, so plans and code get that care on every run.

## 0.9.5

### Fixed
- **Talking it through with the PM reads as one conversation again.** When you discuss the task
  or approve the plan, the PM's answer and your reply now stay together in **Run Conversations**:
  you answer right under the PM's message, and your reply shows once as your message to the PM,
  with your screenshots and what you chose. **Side Conversations** keeps only your @ and /ask chats
  and the permissions agents ask for, with no copies of the discussion.

## 0.9.4

### New
- **What's new, in the app.** When an update is ready, **What's new** shows what's new, improved
  and fixed in it before you install. After it installs, Sinag shows it to you once.

### Improved
- **Sinag notices updates on its own.** It checks when it opens, every 30 minutes while it runs, and
  when you come back to its window, so a new version shows up without you looking for it.

## 0.9.3

### New
- **What you agree is kept.** The PM always asks whether QA should test the work or it's dev work
  only, and writes down what you agreed: what you want, must and must-not, how to tell it's done,
  and your decisions. It sits at the top of the plan card, and the developer and QA work from it.
- **The right skills for each task.** The PM picks skills for every task (design, architecture,
  programming principles, security, testing) and the plan card shows them.
- **One run, several rounds.** Under a finished run, **Add another task to this run** continues the
  same conversation, and History shows it as one run with its rounds.

### Improved
- **The last one to work reports to you:** QA on a tested run, the developer on a dev-only run. The
  report says what was done, what was verified, what wasn't, what needs you and what's next.
- **The developer proves it builds.** Besides its tests, it runs your project's own lint,
  type-check or build commands and says what it ran.

## 0.9.2

### New
- **Talk it through first.** When you press Run, the PM checks your project and tells you whether it
  can be done, what it understood, what each agent would do and what it needs from you, before any
  plan. Turn it off in Settings → Team & runs.
- **Engineering skills on every task:** architecture and feature planning for the PM, test-first
  building and root-cause debugging for the developer, edge cases and security for QA.
- **You see helper agents.** When an agent hands work to a helper agent, you see its job, its
  instructions and every step it takes.

### Improved
- **Safer web access.** Reading a page or searching runs on its own. Anything harmful (running
  downloaded code, sending your data or a login out, saving a download, connecting to another
  computer) asks you first and says what will happen if you allow it.
- **Every change is checked for leaked keys and XSS** before it is tested, without using tokens.

## 0.9.1

### New
- **Side chats have their own tab**, with Open in new tab, Hide and Delete.
- **Discard** on the plan card, and **Skip tests for this run**.
- **Tests tab** with the live test output.
- The side-chat PM can write docs and run setup commands, each with your OK.
- Chat and side chats take documents and video as well as images.

### Improved
- The developer runs the tests for its own change, fixes what fails and runs them again before
  handing over.
- Lower credit use: a passed suite is never run again, and the PM's thinking is capped at medium.

### Fixed
- QA's test commands work with Sinag's own Python.
- An empty UI review no longer sends a finished task back to the developer.
