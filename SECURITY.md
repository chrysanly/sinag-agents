# Security

## Reporting a vulnerability

Please report security problems **privately**, not in a public issue:

1. Open the **[Security tab](https://github.com/chrysanly/sinag-agents/security)** of this
   repository and choose **Report a vulnerability**. Only Chrys can see the report.
2. Say what you found, the Sinag version (shown in the title bar), and the steps to reproduce it.

Chrys aims to reply within a week. A confirmed problem is fixed in a new release, which reaches
every installed copy through the in-app updater. Once the fix is out, you're credited in the
release notes unless you'd rather not be.

**Supported versions:** only the [latest release](https://github.com/chrysanly/sinag-agents/releases/latest)
gets security fixes. Sinag offers each update in Settings, and it installs only when you choose.

## How Sinag protects you

### Your code and your data stay on your PC

- Sinag runs on your computer. Your projects are never uploaded to Chrys or to any Sinag server.
  There is no Sinag server, no tracking and no analytics.
- Run history, settings and screenshots are stored in your Windows profile
  (`%APPDATA%\com.chrys.sinag`). The trial's usage is also recorded in the registry and in
  `%ProgramData%`, so reinstalling doesn't reset it.
- Sinag connects to the internet only for these:

  | Where | Why |
  |---|---|
  | Anthropic, through **your** Claude Code | The agents' work. Handled under your own agreement with Anthropic. |
  | The AI connection **you** choose instead (your Anthropic API key, OpenCode Zen, or a free provider's API) | Only while that connection is the one in use. Your key is encrypted on your PC and sent only to that provider. |
  | `cdn.jsdelivr.net`, `unpkg.com`, `fonts.googleapis.com`, `fonts.gstatic.com` | Only when a designer's mockup uses one of a short list of pinned animation and 3D libraries, or Google Fonts (see below). |
  | `github.com/chrysanly/sinag-agents` | Checking for and downloading signed updates. |
  | `claude.ai/install.ps1` | Only on first setup, and only if Claude Code is missing: Anthropic's official installer. |
  | GitHub, for a project you connect | Only when you press Pull or Push (subscription). |
  | Web pages an agent looks up | Only when an agent reads docs or searches during a run. Harmful calls ask you first (see below). |

### The agents only get the permissions they need

- **Sinag** (planning and talking with you), the **tester** and the **designer** can read the
  project but never change it: their tools are read-only in every mode. Sinag gets the developer's
  permissions only for a small change she makes herself, after you keep **Sinag does this herself**
  ticked and press Begin, and only for that change.
- The **developer** can edit files and run install, test and the project's own check commands
  (lint, type-check, build). Any other command asks you. Risky commands (deleting files, pushing
  code) always ask you first, in every mode, including Auto.
- **Web and network calls are judged before they run, for every agent.** Reading a web page,
  searching, or a plain download that only prints a page runs on its own. Anything harmful asks you
  first and says what it is and what will happen if you allow it: running downloaded code, sending
  your data, a login or a cookie to a site, saving a downloaded file, connecting to another
  computer, an encoded command, installing a package straight from a URL, or an address that carries
  data. This holds whatever a skill or a file in your project tells the agent to do.
- Every change the developer makes is checked by Sinag itself, before it is tested, for leaked keys
  and for XSS (a visitor's input written into the page or run as code, cookies sent out, scripts
  loaded over plain http).
- Sinag never uses Claude Code's "skip all permission checks" mode.
- **Secrets:** no agent can read or change `.env` files, private keys or certificates. The
  developer is told to keep every key and password in `.env` (git-ignored), and every change is
  checked for leaked keys before it is tested.
- Agents reach you only through Sinag's window, over a local connection protected by a random
  token that changes every run.

### Only genuine updates and keys work

- **Updates** are signed with Chrys's private update key. Sinag checks the signature and refuses
  any update that doesn't match, so a changed or fake installer can't be installed through the
  updater.
- **Licence keys** are signed with a separate private key that never leaves Chrys's PC. The app
  only contains the public half, which can check keys but can't make them.
- The bundled Python is Python Software Foundation's official build. Its signature is checked
  when Sinag is built.
- The window only runs Sinag's own code. It loads no scripts from the internet (strict Content
  Security Policy).
- **Designer mockups are locked down.** A mockup is a web page an AI wrote, so Sinag treats it as
  untrusted: before it is saved, every outside address in it is removed except a short list of
  pinned library builds and Google Fonts, and a Content Security Policy is put in the page so the
  browser refuses anything else, even an address its script builds while it runs. It opens in a
  separate preview window that can't call Sinag or reach your files.
- The bundled agent skills are scanned and reviewed before they are included. Nothing is
  fetched at run time.

### The app itself

- A PIN protects opening Sinag. It is stored only as a salted PBKDF2 hash and asked again after
  24 hours, when you sign out, or with **Lock now**.
- Opening a screenshot that an agent looked at is limited to files inside the project, or to
  Sinag's own saved copy.

## What stays your responsibility

- **Review what the agents change** before you deploy it. AI agents make mistakes.
- **Keep your project in git** (or another backup) so any change can be undone.
- **Keep your Claude account safe.** Sinag uses your Claude Code sign-in and never sees your
  password.
- **Download Sinag only from this repository.** Windows may warn about a new app on first
  install. The installer is `sinag-installer.exe` from the
  [releases page](https://github.com/chrysanly/sinag-agents/releases), and you can check its
  SHA-256 against the value in the release notes.
