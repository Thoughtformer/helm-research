# Helm
### Learning how AI-assisted work can remain accountable to people

**An independent, AI-assisted research and engineering project by [Aaron Spoonts](https://thoughtformer.github.io/).**

[Personal portfolio](https://thoughtformer.github.io/) · [Visual project overview](https://thoughtformer.github.io/helm/) · [Research notes](RESEARCH_NOTES.md) · [Milestones](MILESTONES.md)

## Why I am doing this

I am working toward a meaningful career transition into AI-related work. My background spans technical systems, troubleshooting, electronics repair and refurbishment, data, and creative technology. It gives me practical experience with complicated problems, but I am still developing the programming and research skills this field requires.

I tend to stay with a difficult problem, listen to feedback, and keep looking for a workable solution. Helm gives that persistence a direction: learning how AI systems can be useful while remaining understandable, constrained, and answerable to the people using them.

The project began as an attempt to make better use of existing computers and AI tools. Its failures led me toward questions about oversight, authority, verification, and the cost of additional automation. I want to understand those questions through concrete work, and I am looking for opportunities to learn from people with deeper experience.

## What is Helm?

**Helm** is the project name and the human-facing layer. **Escapement** is its underlying control layer, intended to govern execution, approvals, and evidence.

The intended workflow is simple:

**Describe an outcome → inspect the proposed work → approve consequential actions → examine a result with clear limits.**

The implementation is an early prototype. This public repository is a **documentation-only showcase**, not the implementation repository or a runnable evaluation package. The implementation and detailed working records remain private. Public summaries below are drawn from those records and are not independently reproduced by this repository.

## The questions I keep coming back to

**Who decides what an AI system is allowed to do?**  
The model should not be able to grant itself tools or expand its own permissions. I am exploring the separation between proposed work and execution authority.

**What does a person's approval actually authorize?**  
A broad instruction to help is different from approval of a particular consequential action. The design ties approval to the exact proposed content and treats changed proposals as needing review.

**How do we know a task succeeded?**  
A model saying “done,” an HTTP response, a passing structural check, and a useful correct result are different kinds of evidence. The project preserves VERIFIED, UNVERIFIED, and UNKNOWN distinctions.

**Does more orchestration earn its complexity?**  
I want to compare useful outcomes, errors, human effort, calls, latency, and computation under comparable conditions. More agents or more elaborate documentation should not be mistaken for better results.

**Can a non-specialist understand when to trust the system?**  
Oversight depends on what a person can understand from the interface, including uncertainty, permission scope, incomplete outputs, and failure.

## What the work has surfaced so far

| Observation from the project record | Why it matters | Limit |
| --- | --- | --- |
| A functioning control/execution path did not establish general worker competence. | The runtime and the worker need separate evaluation. | This concerns bounded development work, not a general result about model ability. |
| A planning request ended at its output limit without a usable plan. | Incomplete output must remain visibly incomplete. | Later synthetic tests did not establish successful live planning. |
| Early workflow comparisons had unequal tool access and narrow fixtures. | A useful-looking advantage can have a confounded explanation. | No broad superiority or economic savings claim is supported. |
| Installer and application-control problems remained despite passing focused tests. | Passing a test suite is not the same as an independently usable product. | Owner acceptance and wider readiness remained unverified. |

[Read the case notes and their evidence boundaries →](RESEARCH_NOTES.md)

## My contribution, and where AI helps

I direct the project, define goals and constraints, review proposed decisions, try workflows, identify problems, and guide revisions. My technical background helps me ask practical questions and persist through troubleshooting.

AI tools contribute substantially to implementation, investigation, and writing—including this presentation, which was prepared with AI assistance under my direction. I do not claim to have independently written every line or to have established research expertise from owning the repository.

The private implementation also reuses upstream software, including StarNet. This showcase does not claim that reused components are original work or publish their source under a new license.

## Where I want to grow

I am continuing to develop Python, experiment design, evaluation methods, security fundamentals, and my understanding of AI governance and safety. I want to get better at forming testable questions, distinguishing evidence from a persuasive explanation, and accepting results that challenge my assumptions.

My aim is to become useful in this field through careful work, a willingness to listen, and sustained learning. Helm is a record of that effort, not a claim that the learning is finished.

## Current boundaries

This is exploratory work, not a finished safety system, peer-reviewed publication, compliance certification, or production-ready general agent platform. Project readiness remains unknown; adaptive routing is not qualified. Proposed future studies are not completed experiments. Avoid inferring implementation coverage or reproducibility from this public documentation alone.

**Last editorial update: October 18, 2026.** Historical milestones retain their original dates; no new experiment was run for this publication.
