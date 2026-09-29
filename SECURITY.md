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
  | `github.com/chrysanly/sinag-agents` | Checking for and downloading signed updates. |
  | `claude.ai/install.ps1` | Only on first setup, and only if Claude Code is missing: Anthropic's official installer. |
  | GitHub, for a project you connect | Only when you press Pull or Push (subscription). |

### The agents only get the permissions they need

- The **PM** and **QA** can read the project but never change it: their tools are read-only in
  every mode.
- The **developer** can edit files and run install and test commands. Any other command is
  refused. Risky commands (deleting files, pushing code, downloading) always ask you first, in
  every mode, including Auto.
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
