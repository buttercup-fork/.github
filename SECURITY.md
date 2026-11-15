# Security policy

This policy covers every repository of [buttercup-fork](https://github.com/buttercup-fork), CodeKunde's fork of the Buttercup password manager. The original Buttercup project is no longer maintained and is not part of this fork: please do not send reports about this code to it.

## Reporting a vulnerability

Report it privately. Do not open a public issue or pull request.

- **On GitHub:** the **Report a vulnerability** button on the repository's **Security** tab.
- **By email:** [buttercup@codekunde.net](mailto:buttercup@codekunde.net)

Please include:

- the component and its version or commit
- your operating system, and your browser if it matters
- the steps to reproduce it
- what an attacker gains

Never send a real vault, an export or a real password. A test vault with a test password is fine.

## What to expect

These are the targets we work to. If we can't meet one, we tell you and say when to expect an answer.

- **Acknowledgement:** we aim to reply within 7 days. If you have heard nothing after 7 days, please send the report again: mail can get lost.
- **Assessment:** we aim to tell you within 14 days whether we could reproduce the issue and how severe we rate it. Anything that could expose vault contents or the master password without the user's help goes to the front of the queue.
- **Fix:** our targets depend on the severity, counted from when we reproduce the issue: critical within 7 days, high within 30 days, medium within 90 days or by the next release.
- **Credit:** in the advisory and the changelog, under the name you choose, if you want it.

## Disclosure

Please keep the details private until a fixed release is available, or until 90 days after your report, whichever comes first. If we need longer, we will ask you before the 90 days are up and tell you why.

We publish a GitHub security advisory for every fixed vulnerability of medium severity or higher that reached a release.

## Safe harbour

If you research this fork in good faith, we will not bring legal action against you for that research, will not refer it to law enforcement, and will not voluntarily support anyone else who does. Good faith means that you:

- test only against your own installation, vaults and accounts;
- do not access, change, keep or share anyone else's data, and if you reach it by accident, stop, delete what you have and tell us;
- do not degrade a service other people use;
- follow the Disclosure section above and do not ask for payment in return for not disclosing.

You may share details earlier with the National Cyber Security Centre or the maintainer of an affected dependency, if you tell us who. This commitment covers research done while this version of the policy is published and binds anyone who later owns this fork. It does not bind anyone else, including Dropbox, Google, Microsoft, the authors of the original Buttercup project or other contributors, and it does not make lawful anything that is otherwise unlawful.

You are responsible for complying with the law where you are. If you are unsure whether something is covered, ask us first at [buttercup@codekunde.net](mailto:buttercup@codekunde.net).

## Supported versions

Security fixes go into the latest release of each component. A component this fork has not released yet gets them on its `master` branch.

## Scope

**In scope:**

- the desktop app, the browser extension and the core library
- the libraries this fork maintains: the importer, exporter, generator, locust, file-interface, fetch, channel-queue, google-oauth2-client, and the Dropbox, Google Drive and OneDrive clients
- the command-line tool and the mobile app, once they are released
- a flaw in a dependency, when Buttercup's use of it can reach it

**Out of scope:**

- CodeKunde's websites and email servers
- Dropbox, Google, Microsoft and WebDAV servers themselves
- the original project's unmaintained packages
- weak master passwords
- an attacker who already controls the unlocked device
- social engineering of the maintainer
- denial of service by traffic volume

## How this code is checked

Before the first release, the core library, the browser extension and the desktop app's main process were reviewed with Cloudflare's [security-audit-skill](https://github.com/cloudflare/security-audit-skill) (commit `c1c8a8c`), an AI-assisted review tool, run in an isolated sandbox. The maintainer checked each of its findings before acting on it. The other components were reviewed by the maintainer with AI-assisted tools.

None of this is a third-party audit, and the code has not had one.
