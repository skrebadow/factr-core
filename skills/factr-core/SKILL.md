---
name: factr-core
description: Apply behavioral falsifiability when deriving or assessing software behavior, acceptance criteria, tests, or automation from engineering context. Use available sources and bounded inference to produce traceable, challengeable results. Applies to FACTR Core requests; installation alone does not select a task or authorize actions.
---

# FACTR Core

Behavioral reasoning contract, version 0.1.0. Behavioral falsifiability is the reasoning engine. Interpret, derive, assert, challenge, apply, trace, and qualify are interleaved reasoning operations, not stages to invoke or artifacts to generate.

## Serve the requested outcome

Use supplied conversation, documents, diagrams, code, tests, and observations as working context. Informal descriptions can support exploration. Source authority is relevant to accepted obligations and formal conclusions; it is not a prerequisite for candidate assertions or test design. Reuse information already supplied.

Deliver the requested requirements analysis, epic, feature, story, acceptance criteria, assessment, test strategy, test case, automation, or traceability result. Combine outputs when requested. Use plain engineering language; introduce FACT terminology only when it helps or is requested. Do not require a stage selection, preflight artifact, approved claim, separate FACT Set, or intermediate schema to reason.

## Expose and challenge behavior

Identify relevant subjects, conditions, responsibilities, interactions, state changes, boundaries, and meaningful failure possibilities. Distinguish source statements from useful engineering implications. Preserve explicit constraints. Do not invent established obligations, actors, interfaces, thresholds, or implementation details to make an assertion look concrete.

For each relevant assertion, retain recoverable anatomy:

- **Subject:** entity responsible for the behavior.
- **Condition:** input, trigger, state, or boundary that scopes it.
- **Behavior:** one independently challengeable commitment.
- **Observable outcome:** direct result an appropriate observer can distinguish.

Identify the contrary observation that would disprove it and a suitable observation target. If one commitment could hold while another fails, split them. Keep useful direct baselines and add grounded implications where available. Generate only the assertions the behavior warrants. A vague capability with a generic “works correctly” outcome is not falsifiable.

Choose the smallest verification boundary that can challenge the behavior. Inspection, analysis, unit checks, integration tests, demonstrations, and operational observation may each be appropriate; do not assume every assertion requires a UI, consumer, end-to-end test, or automation.

## Continue with bounded uncertainty

When the input supports a useful answer, proceed. When it supports only provisional reasoning, state material assumptions and deliver defensible candidates. When interpretations conflict, preserve them separately and offer common behavior or conditional tests that distinguish them. Do not silently select an interpretation.

Ask a clarifying question only when missing information prevents a meaningful requested answer. Explain exactly which conclusion cannot be determined and why, while delivering the limited analysis that remains possible. Missing runtime access prevents an executed verdict, not test design. Unknown interface bindings can remain explicit in automation design; they cannot be presented as established runnable bindings.

## Keep support, observations, and decisions separate

Use these independent concepts where material:

- **Support:** explicit in supplied context; inferred with a defensible basis; or proposed for investigation. A proposed behavior is not a requirement.
- **Unknowns:** parameters or decisions that affect conditions, scope, expected results, or failure interpretation. Preserve the weakest material assumption in a mixed-support assertion.
- **Potential evidence:** an observation target or verification plan.
- **Actual evidence:** a supplied or collected record, with source and relevant target, conditions, version, and limitations when available.
- **Evaluation:** not evaluated, supported within observed scope, contradicted within observed scope, or inconclusive.
- **Formal acceptance:** a separate decision under applicable criteria and review policy.

An explicit assertion may be contradicted by observed evidence. An observed proposed behavior does not thereby become an obligation. Never label an expected result, inferred implementation, or suggested probe as observed. Missing or unusable observation is inconclusive unless absence under a defined condition and observation window is itself the established falsifier. A passing test supports its tested scope; it does not prove universal requirement satisfaction.

## Apply and preserve meaningful links

For every generated test, retain an identifiable assertion, relevant conditions, expected observation, and failure condition. Preserve supplied requirement IDs and source locators; use lightweight local references when needed. Link inferences to their premises and material assumptions. Link actual results to the assertion and conditions they address.

Use as much trace detail as the task needs. A clear sentence can hold the anatomy; a standalone claim table is optional. One assertion can have several tests; one scenario can challenge multiple assertions if its observations are separately attributable. A link alone does not establish coverage. State reviewed scope and exclusions before claiming completeness.

Preserve source quotations and prior accepted baselines without freezing the working model. When new information changes meaning, revise affected assertions and tests, retain relevant history, and identify conclusions that need reassessment. For saved or multi-turn work, keep material bases, assumptions, and links in the deliverable or requested structured export; hidden chat context must not be their sole durable record.

## Formal conclusions and optional capabilities

For compliance, certification, formal baseline acceptance, or definitive verification, read [formal-verification.md](references/formal-verification.md) and apply supplied criteria and policy. Missing authority, evidence, or sign-off limits that conclusion; continue useful exploration. Ordinary trace mapping does not require this reference.

Use existing tools only when needed to read additional sources, create requested files, inspect supported bindings, or perform authorized execution. Mark illustrative or incomplete code accordingly. Correctness of a claim, approval of a baseline, and authorization to use a tool are separate. Do not invoke existing FACTR stages or import their governance merely because Core is active. Do not run development checks or load evaluation material during ordinary reasoning.

**Operating rule:** Reason first. Challenge behavior. Preserve uncertainty. Deliver useful results.
