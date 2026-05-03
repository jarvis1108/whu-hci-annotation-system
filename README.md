# Web-based Text Annotation System

<img width="1536" height="1024" alt="Interface concept reconstruction" src="https://github.com/user-attachments/assets/95b8c4ee-eec6-46f4-8d9f-e15e7f4e7834" />
</br>

*Concept reconstruction of the main labeling screen — original deployment screenshots no longer available.*

A web-based annotation tool built for the **Wuhan University HCI Lab** to support crowdsourced research data collection. Reached **1,000+ active users** during operation.

> Built 2019. README written 2026 to add documentation context — code itself unchanged from the original 2019 push. Archived; not maintained.

## What it did

Researchers uploaded text passages requiring human review. Crowd workers logged in, were served passages one at a time, made a binary judgment, and (when flagging) drag-selected the specific evidence in the text. The system tracked per-user deadlines, per-task time costs, and exported labeled datasets back to researchers.

## Tech stack

- **Frontend**: JSP + JSTL templates · Amaze UI 2.x (Bootstrap-equivalent for the Chinese ecosystem) · jQuery 3.4.1 (slim build)
- **Backend**: Java Servlet API · custom session handling for per-user task queues + deadlines
- **Database**: MySQL (passage corpus, user accounts, label submissions with timing data)
- **Build**: IntelliJ IDEA artifact deploy to Tomcat

## Why it's still here

This was my first time owning a real product end-to-end — UI design, frontend, servlet backend, schema design, user testing. The decisions weren't perfect (today I'd reach for React + a typed backend + Postgres), but the system shipped, served real research, and taught me what *implementation reality* feels like at the design layer.

That experience is the through-line into my current work designing enterprise systems for [NYC Public Schools](https://huchongjin.com), where understanding the production codebase is part of the design job.

## Status

Archived 2026 — the lab transitioned to a different platform. Kept public as engineering background reference.
