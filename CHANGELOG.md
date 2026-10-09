# What's new in Sinag

Sinag shows the newest section before it updates (Settings → **What's new**) and once after.

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
