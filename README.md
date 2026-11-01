# FACTR Core

Version 0.1.0. Reason about what software should do, how it could fail, and how to test it from the information available.

FACTR Core is the maintained plugin for this project, with one behavioral reasoning contract. It preserves falsifiable assertions, bounded inference, and claim-level traceability without requiring stage invocation, approved intermediate artifacts, or a separate FACT Set for each task.

## Start using the methodology

The runtime contract is [SKILL.md](skills/factr-core/SKILL.md). Example requests:

- “Design tests from this feature description; label material assumptions.”
- “Draft a story, acceptance criteria, and tests from these notes.”
- “Assess which behavioral failures these existing tests can detect.”
- “Compare these conflicting interpretations and propose discriminating tests.”

Outputs distinguish explicit expectations, inferences, proposals, unknowns, and actual observations. A candidate assertion may guide test design before formal acceptance. Missing runtime evidence does not prevent designing a test. Formal conclusions use the conditional [verification profile](skills/factr-core/references/formal-verification.md).

## Installation

You need Git, Bitbucket access (corporate network/VPN if required), and [Codex CLI](https://developers.openai.com/codex/cli) for registration. Install through a signed-in Codex desktop app or CLI. FACTR Core requires no build or additional runtime dependencies.

### 1. Register the marketplace

Run in PowerShell from your projects directory:

```powershell
git clone "https://lnsvr0329.gcsd.harris.com:8443/bitbucket/scm/factr/factr-core.git" factr-core
Set-Location -LiteralPath .\factr-core
codex plugin marketplace add .
```

Already cloned? Enter the repository root and run only the registration command.

Alternatively, register Bitbucket directly without a local checkout:

```powershell
codex plugin marketplace add "https://lnsvr0329.gcsd.harris.com:8443/bitbucket/scm/factr/factr-core.git" --ref main
```

### 2. Install and enable

**Desktop:** Open the local checkout as a project if applicable. Restart the app, open **Plugins**, select the **FACTR Core** marketplace, and install and enable **FACTR Core**.

**CLI:** Launch Codex:

```powershell
codex
```

Inside the interactive session, enter:

```text
/plugins
```

Select the FACTR Core marketplace, install its plugin, and ensure it is enabled.

### 3. Start using FACTR Core

Start a **new chat or CLI session** after installation. Confirm the plugin browser shows FACTR Core installed and enabled. Select it with `@` in the desktop composer, or invoke its CLI skill:

```text
Use $factr-core to propose acceptance criteria and tests from this description.
```

### Updates and troubleshooting

For a local checkout, run `git pull --ff-only` first. Then refresh either source:

```powershell
codex plugin marketplace upgrade factr-core
```

Restart the host and start a new session. If the source is missing, verify you registered the repository root containing `.agents/plugins/marketplace.json`. For installation or policy issues, consult the [official plugin guide](https://developers.openai.com/codex/plugins).
