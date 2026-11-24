## Buttercup: a free, open-source password manager

Buttercup keeps your passwords in an encrypted vault that only you can open. The original project was archived and no longer gets fixes; this is CodeKunde's independent continuation of it, not affiliated with the original maintainers. Breathing life into the Buttercup that [Perry Mitchell](https://perrymitchell.net/projects) made.

**3.0.0 / 4.0.0 (2026-11-24) fix security problems in the original Buttercup apps.** What to do: [release notes](https://github.com/buttercup-fork/buttercup-desktop/releases/tag/v3.0.0).

**Get Buttercup:** [buttercup.codekunde.net](https://buttercup.codekunde.net/)

| Repository | What it is |
| --- | --- |
| [buttercup-desktop](https://github.com/buttercup-fork/buttercup-desktop) | The desktop app for Windows and Linux ([releases](https://github.com/buttercup-fork/buttercup-desktop/releases)) |
| [buttercup-browser-extension](https://github.com/buttercup-fork/buttercup-browser-extension) | The extension for Chrome and Firefox; works together with the desktop app |
| [buttercup-core](https://github.com/buttercup-fork/buttercup-core) | The library that reads, writes and encrypts vaults |

The other repositories are the libraries behind them: cloud storage and sign-in clients, import and export, the password generator and the extension's login-form finder. `secure-file-host` is kept for reference; the desktop app no longer uses it.

**Questions and ideas:** [Discussions](https://github.com/orgs/buttercup-fork/discussions). **Bugs:** an issue in the app's repository.

**Security problems:** please report them privately, as the [security policy](https://github.com/buttercup-fork/.github/blob/master/SECURITY.md) describes. Nobody from Buttercup will ever ask for your master password or a vault file.
