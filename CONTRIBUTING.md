# Contributing to the Distributed Diagnostics Program

Thank you for your interest in contributing to the Spaghetti Table Protocol Challenge. This document explains how to participate.

---

## Who Should Contribute

- Design researchers and educators
- HCI researchers and practitioners
- AI safety researchers
- Anyone with access to a multimodal AI system and 15 minutes

No prior AI research experience required. No Python required. No institutional affiliation required.

---

## How to Contribute

### Option 1: Run the Protocol and Submit Results

This is the primary contribution. Administer the Spaghetti Table Protocol to any multimodal AI system, score your results, and submit.

**Steps:**

1. Read the [Protocol Specification](protocols/spaghetti-table-protocol-v1.md)
2. Administer the two prompts to any multimodal AI system
3. Score the outputs using the three-pillar rubric
4. Complete the [Submission Template](submissions/submission-template.md)
5. Submit via one of the three methods described in the template

**Time required:** 15–30 minutes per system tested.

---

### Option 2: Design New Failure-Inducing Prompts

The Spaghetti Table is one diagnostic scenario. The design community has the spatial intelligence, material knowledge, and scenario design skills to develop an entire battery of failure-inducing prompts.

A strong failure-inducing prompt:
- Places objects in physically impossible relationships that the AI cannot retrieve from training data templates
- Simultaneously stresses at least two of the three pillars
- Produces a physically determinate scenario that can be scored against the rubric
- Is novel enough to prevent template retrieval while concrete enough to produce a scorable output

If you design a new scenario that reliably elicits Inversion Error failures, submit it as a prompt proposal by opening a GitHub Issue with the label `new-prompt-proposal`.

---

### Option 3: Extend the Rubric

If you administer the protocol and observe failure modes that fall outside the current three-pillar rubric, document them in the Open Exploration Notes section of your submission. Failure modes that appear consistently across multiple submissions become candidates for inclusion in future protocol iterations.

---

### Option 4: Translate the Protocol

If you administer the protocol in a language other than English, or across non-English AI systems, your results are particularly valuable for establishing cross-linguistic generalizability of the three-pillar diagnosis. Note the language of administration in your submission.

---

## Submission Guidelines

- Anonymous submissions are accepted
- Modifications to the standard prompts must be noted
- All submitted data will be included in the aggregate dataset under CC BY 4.0
- Submitters retain attribution rights

---

## Code of Conduct

This is a collegial research community. Contributions are reviewed in the spirit of open science. Critique of AI systems is the point; critique of contributors is not.

---

## Questions

Open a GitHub Issue or email pzakrzewski@tru.ca

---

## License

All contributions to this repository are licensed under  
[Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/)
