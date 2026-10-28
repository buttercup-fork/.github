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

One person maintains this fork in their spare time, so we promise only what one person can keep:

- **Acknowledgement within 7 days.** If you have heard nothing after 7 days, send the report again: mail can get lost.
- **An assessment within 3 days** for anything that could expose vault contents or the master password without the user's help, and **within 14 days** for everything else. The assessment says whether we could reproduce it, and how severe we rate it.
- **A fix target that depends on the severity,** counted from when we reproduce it: critical within 7 days, high within 30 days, medium within 90 days or the next release.
- **Credit** in the advisory and the changelog, under the name you choose, if you want it.

## Disclosure

Please keep the details private until a fixed release is available, or until 90 days after your report, whichever comes first. If we need longer, we will ask you before the 90 days are up and tell you why.

We publish a GitHub security advisory for every fixed vulnerability of medium severity or higher that reached a release.

## Supported versions

Security fixes go into the latest release of each component. A component this fork has not released yet gets them on its `master` branch.

## Scope

**In scope:**

- the desktop app, the browser extension and the core library
- the libraries this fork maintains: the importer, exporter, generator, locust, file-interface, fetch, channel-queue, google-oauth2-client, and the Dropbox, Google Drive and OneDrive clients
- the command-line tool and the mobile app, once they are released
- a flaw in a dependency, when Buttercup's use of it can reach it

**Out of scope:**

- Dropbox, Google, Microsoft and WebDAV servers themselves
- the original project's unmaintained packages
- weak master passwords
- an attacker who already controls the unlocked device
- social engineering of the maintainer
- denial of service by traffic volume

## How this code is checked

The code is reviewed with AI-assisted tools and by the maintainer. It has had no third-party audit.
