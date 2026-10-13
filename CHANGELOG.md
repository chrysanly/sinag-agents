# What's new in Sinag

Sinag shows the newest section before it updates (Settings → **What's new**) and once after.

## 0.11.1

### New
- **The team works side by side.** Tala fixes what Liwanag or Bahaghari send back straight away,
  while she builds the next task, so a bug never waits behind new work. Bahaghari designs the next
  screens while she checks finished ones, and Tala builds whatever is ready instead of waiting for
  a design to be approved.
- **Choose which screens Bahaghari designs first.** The plan card lists every screen she would
  design, each with its own switch. Turn one off and Tala builds it straight from the plan.

### Improved
- **Pause stops now.** Pausing an agent stops its current step at once instead of letting it
  finish first. **Resume** carries on from exactly where it stopped, with nothing redone.
- **The conversation shows the run you're on.** Earlier runs stay in History, so opening a project
  or continuing a run is quick, with no long scroll to the bottom. Each project also remembers
  where you were reading.

### Fixed
- **Continue where it left off no longer starts over.** Tasks that were already built go straight
  to their check, a task sent back for a fix keeps what to fix, and designs you approved are built
  without being designed or approved again. This saves a lot of usage when a run stops, for
  example at your Claude usage limit.
- What you and Sinag agreed is kept when a run continues.

## 0.11.0

### New
- **Sinag leads the team.** Sinag herself now talks the work through with you, writes the plan and
  hands it to the team, in place of Ray. Ask her anything in a side conversation with **@Sinag**.
  Your own names for the team still work.
- **Sinag does small changes herself.** When a change is small, the plan says so and **Sinag does
  this herself** starts ticked: she makes the change and runs your tests, with no other agent, so
  it's quicker and uses fewer tokens. Untick it and the team does it.
- **Bahaghari designs first.** For every task that changes what you see, Bahaghari now makes a
  mockup of the finished screen before anything is built, in your project's own colours and fonts,
  with screenshots on desktop and phone. **Approve** it, or type what to change and press **Change
  it** for a new version. Tala builds to the design you approved, and Bahaghari checks the result
  matches it before it's tested. (With a subscription.)
- **Open live.** Open Bahaghari's mockup itself, not just its screenshots: hover, click, watch the
  motion and resize it to phone width. It stays with the run, so it opens from History too.

### Improved
- **Sharper design and engineering skills.** Bahaghari and the team check every screen against
  craft rules that avoid the generic "AI-made" look, use the right tool for animated characters, 3D
  and scroll-told pages when a task needs them, and write secure code by default (checked input and
  access, safe and fast queries, the right tests) on any stack.
- **Mockups are locked down.** A mockup may only load a short list of trusted animation libraries
  and Google Fonts. Everything else is blocked, so a design can't reach anything it shouldn't.
- **Settings → Plan lists everything a subscription adds**, including the designer, Learn with
  Luna, the extra styles and your own wallpaper.

### Fixed
- The Design tab scrolls again when it holds more reviews than fit.
- Side Conversations no longer says "No questions in this run yet" while a question is waiting for you.

## 0.10.0

### New
- **Bahaghari, the designer.** A fourth member of the team. After Tala builds a task that changes
  what you see, Bahaghari looks at the real app on desktop and phone and checks the look, the feel
  and the motion: layout and spacing, type, colour and contrast, every state, animations and the
  phone layout. What isn't right goes back to Tala to fix before QA tests it, so QA can focus on
  whether everything works. With QA off, Bahaghari reports to you.
- **The Design tab.** See every design review in the Desktop view: the verdict for each task and
  round, what had to be fixed, ideas for you, and the screenshots Bahaghari judged. Open any of
  them big. The reviews show in the conversation too.
- **Sinag runs your app for the team.** For work on a web project, Sinag starts the project's own
  dev server in the background, with no command window, tells the team its address and stops it
  when the work is done. Open it yourself from the Design tab.
  The designer comes with a subscription. Turn it on or off in Settings → Team & runs → Design
  check, and rename it like the others.

### Improved
- The team names the designer in its plans: the PM marks which tasks change what you see.

## 0.9.9

### New
- **Luna, your mentor.** Learn now has a mentor of its own. Luna writes your learning paths and
  sits in her own sidebar: ask her about a step, let her check your work, fix it or build it in your
  practice project. She teaches at a senior level and never sends you off to read the docs. Her
  notes stay with Learn and never reach the team.
- **Choose where Sinag's AI comes from.** Settings → Usage: your Claude plan through Claude Code,
  your own Anthropic API key, OpenCode Zen credits, or Free usage (Gemini, Groq, OpenRouter and
  OpenCode's free models). Connect each once, switch whenever you like, and every option says
  plainly whether it is free or paid. "How usage works" explains them all.
- **No Claude login needed to open Sinag.** Your PIN opens it. Claude only asks you to sign in when
  Claude Code is what you use.
- **AI in use, always visible.** The account chip and Settings → Account show what Sinag runs on
  now, with a switch. The chat, the team and Luna each show their connection, model and effort.
- **Basic or Pro paths.** Pro covers a senior full-stack curriculum: standards, architecture,
  security, performance, testing and delivery. Your goal is now binding: what you leave out stays out.
- **Sinag and the team come alive.** New animated characters for Sinag, Luna, Ray, Tala and
  Liwanag, and a new Sinag on the splash screen, the sign-in screen, the title bar and the app icon.

### Improved
- **Paths keep writing in the background.** Write several at once, keep using Sinag, and see them
  appear even after a reload.
- **Models follow your connection.** The model lists show the models of what you use, and effort
  only appears where it applies.
- **The chat is now Chat with Sinag.**
- **Learn setup steps** include their full configuration, and the practice folder can be picked
  when you start a path.

### Fixed
- **A usage limit no longer loses a path.** Luna pauses and continues from exactly where she
  stopped, on any connection you choose.
- Code in learning steps shows properly.
- Toggles in Settings line up.

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
