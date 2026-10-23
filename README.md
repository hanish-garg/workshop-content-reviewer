# Workshop Content Reviewer (Kiro Power)

A Kiro power for reviewing AWS Workshop Studio lab content for any service or topic before it is merged. It checks structure, front matter, Workshop Studio directives, code blocks, images, links, prerequisites, security, content quality, cleanup, `contentspec.yaml`, and AWS Well-Architected alignment, then writes a `Review.md` report.

## Contents

| File | Purpose |
|------|---------|
| `POWER.md` | Power metadata, Step 0 (discover house conventions), universal patterns, Well-Architected guidance, common issues |
| `steering/review-checklist.md` | Checklist sections A–P, domain modules, severity guide, and the `Review.md` template |

## How it works

1. **Step 0:** Sample existing labs in the target workshop to learn its house conventions (weights, prerequisites format, cleanup model, code block style).
2. **Checklist:** Apply universal rules strictly. Judge *(house)* items against the detected conventions.
3. **Domain modules:** Add targeted checks for the lab's area (databases, serverless, containers, compute/networking, analytics, AI/ML, security, developer tooling).
4. **Report:** Write `Review.md` with Critical / Warning / Recommendation findings, each with a file reference and a suggested fix.

## Installation

In Kiro, open the Powers panel and add this power from its local folder or Git repository URL.

## Usage

Ask Kiro something like:

- "Review the new lab in `content/3-Advanced/MyLab` using the workshop content reviewer power."
- "Check this PR's workshop content against workshop standards and write Review.md."
