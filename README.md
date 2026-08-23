# Salesforce Identity & Security Administration — Training Module

A Udemy-style, self-paced training module for the **Salesforce Platform Administrator (CRT-101)** exam,
focused on **Identity & Security Access**: users, authentication/MFA, profiles, permission sets,
roles, org-wide defaults, and sharing rules.

Live site: https://manicminerwd.github.io/salesforce-admin-training/

## What's inside

- Collapsible **curriculum sidebar** with sections and lessons
- **Progress tracking** (localStorage) and a completion bar
- **Lesson pages** with explanations, exam-pattern callouts, and inline **SVG diagrams** of:
  - the authentication layer (login hours / IP ranges / MFA)
  - profiles vs permission sets (additive layering)
  - the role hierarchy
  - org-wide defaults + sharing rules (record visibility)
- A **scenario walkthrough** and an **exam checklist**

## Adding the videos

Each lesson has a video slot. To populate one:

1. Drop your clip at `assets/<lesson-id>.mp4` (e.g. `assets/profiles.mp4`), **or**
2. Set a source in `index.html` by adding a `VIDEO_SOURCES` map near the bottom of the script:

```js
window.VIDEO_SOURCES = {
  profiles: "assets/profiles.mp4",                 // local file
  roles:   "https://www.youtube.com/embed/XXXXXXX" // or a YouTube embed URL
};
```

The player auto-detects `.mp4` vs a YouTube embed and renders the right element.
Until a source is set, the slot shows a placeholder so the layout is complete.

> Note: this module was built without generated video because no text-to-video
> tool was available at build time. The slots are ready for you to drop real
> screen-recordings (or AI-generated clips) in later.

## Not official training

Self-made study companion, not an official Salesforce course. Pair with Trailhead
and the official Exam Guide: https://help.salesforce.com/s/articleView?id=005298966

## Run locally

Just open `index.html` in a browser — no build step.
