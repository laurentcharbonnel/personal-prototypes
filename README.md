# Personal Prototypes

Reusable operating guides for personal experiments. Keep prototype code in dedicated repositories.

## Work → GitHub → Codex

1. **Frame in ChatGPT Work:** Define the hypothesis, constraints, one observable success criterion, and the smallest demonstrable scope. Avoid long specifications.
2. **Prepare a dedicated GitHub repository:** Add a short README, a concise spec, and representative sample inputs. Keep personal playbooks here, not in the professional architecture-skills repository.
3. **Build with Codex:** Open the prototype repository and invoke the reusable `rapid-prototype` skill when available. Implement the minimum working experiment, run focused tests, and report actual results.
4. **Review:** Inspect the running prototype and its evidence. Iterate narrowly, stop, or decide to develop a production solution.
5. **Record:** Keep run instructions, observed outcomes, limitations, and next steps in the prototype repository.

### Reusable Codex prompt

```text
Use the rapid-prototype skill in Technical POC mode, if installed.
Read README.md and spec.md in this repository.
Implement only the agreed minimal scope and its focused tests.
Use existing dependencies when possible; minimize files, cost, and context.
Run the checks and report actual results, limitations, and reproduction steps.
Do not deploy, introduce production architecture, or refactor unrelated code.
```

### Before each experiment

Confirm the hypothesis, target environment, 1–3 representative cases, acceptance criteria, repository visibility, and whether private credentials or company information are involved. Never put confidential data or credentials in a public repository.

## Current experiment

[UI Test Automation](https://github.com/laurentcharbonnel/ui-test-automation): generic YAML-driven browser tests with Playwright against a Vue.js demo. The initial runner requires no LLM calls at execution time.
