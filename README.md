# Salesforce Platform Administrator — Training Module

A Udemy-style, self-paced training module covering the **full Salesforce Certified Platform
Administrator (CRT-101)** exam scope across all **8 domains** (63 lessons).

Live site: https://manicminerwd.github.io/salesforce-admin-training/

## Curriculum (full CRT-101 scope)

1. **Configuration & Setup (15%)** — exam overview, users & MFA, profiles & permission sets, roles/OWD/sharing, company/fiscal/currency, audit trail & sandboxes.
2. **Object Manager & Lightning App Builder (15%)** — objects & fields, relationships, formula & roll-up fields, validation rules, record types & business processes, page layouts, Lightning App Builder.
3. **Sales & Marketing (10%)** — leads, accounts/contacts/opportunities, products & price books, campaigns, forecasting & territories.
4. **Service & Support (10%)** — cases & support process, case automation, entitlements/SLAs, Knowledge, macros & Service Console.
5. **Productivity & Collaboration (10%)** — Chatter, mobile app, activities/actions, AppExchange & packages.
6. **Data & Analytics (17%)** — import/export, duplicate management, reports, dashboards, advanced reporting, list views.
7. **Automation (15%)** — overview & order of execution, Flow Builder, record-triggered flows, approvals, legacy automation, default user & troubleshooting.
8. **Agentforce (8%)** — what it is, Agent Builder (topics/actions), permissions/testing/deployment.

## Features

- Collapsible curriculum sidebar, progress bar + per-lesson completion (localStorage)
- Inline **SVG diagrams** for the key concepts (access model, relationships, formulas, sales/service paths, reports/dashboards, flows)
- Exam-pattern callouts throughout
- **Video slots** in every lesson (see below)

## Adding the videos

Each lesson has a video slot. To populate one:

1. Drop your clip at `assets/<lesson-id>.mp4` (e.g. `assets/profiles.mp4`), **or**
2. Set a `VIDEO_SOURCES` map near the bottom of the `<script>` in `index.html`:

```js
window.VIDEO_SOURCES = {
  profiles: "assets/profiles.mp4",                  // local file
  roles:    "https://www.youtube.com/embed/XXXXXXX" // or YouTube embed
};
```

The player auto-detects `.mp4` vs YouTube embed. Until a source is set, the slot shows a placeholder.

> Note: this module was built without generated video (no text-to-video tool was
> available at build time). The slots are ready for you to drop real
> screen-recordings or AI-generated clips in later.

## Not official training

Self-made study companion, not an official Salesforce course. Pair with Trailhead
and the official Exam Guide: https://help.salesforce.com/s/articleView?id=005298966

Open `index.html` in a browser — no build step.
