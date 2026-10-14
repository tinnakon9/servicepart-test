# AGENTS.md

<!-- init-project:start -->
## Project

- **Name:** ISZT-ServiceParts
- **Purpose:** ระบบจัดการอะไหล่ (Service Parts) แบบ Java multi-module (Eclipse) ครอบคลุมงานรับ ASN, delivery tag report และการค้นหา order
- **Stack:** Java 1.8, Struts 2.2.1, Hibernate 3.3.2, Spring 2.5, JSP, JasperReports 4.0.0, jQuery 3.7.1, SQL Server, Tomcat; ไม่มี Maven/Gradle/Ant ใช้ Eclipse `.classpath` และ jar ใน `app/ServicePartLib`; ไม่มี test suite, lint หรือ CI
- **Modules (`app/`):** `ServicePartWeb` (Struts/JSP), `ServicePartModel` (Hibernate), `ServicePartCommon`, `ServicePartJob`, `ServicePartFH`, `MergeFile`, `ServicePartLib` (jar)
- build และ run ผ่าน Eclipse ไม่มีคำสั่ง CLI; โค้ดต้องคอมไพล์ที่ระดับ Java 1.8
- ห้ามคัดลอกค่าการเชื่อมต่อฐานข้อมูลจาก `hibernate.properties` หรือ `hibernate.cfg.xml` ลงเอกสารหรือ KB

## Project knowledge base

- **Folder:** `knowledge-base/` — an OKF (Open Knowledge Format)
  bundle. Start at `knowledge-base/index.md` for the concept
  listing; `knowledge-base/log.md` holds its change history and
  `knowledge-base/kb-maintenance.md` the rules for adding to it.

บรรทัดด้านล่างคัดลอกมาจาก skill init-project แบบตรงตัวเป็นภาษาอังกฤษ ห้ามแก้ไขหรือแปล
## Working rules

- Start at this project's knowledge base index and open only the concepts
  the task needs; research externally only when the knowledge base does not
  already have the answer.
- After finishing any piece of work, update the knowledge base with what
  changed.
- When you learn something new about this project while working, capture it
  in the knowledge base — don't let it evaporate at the end of the session.
- When a knowledge source outside this repository has its own index (an OKF
  bundle, an LLMWiki, or similar), reference it by index + link and pull in
  only the excerpts you need — never copy it wholesale.
- Keep this file and its adapters current, but edit outside the
  `init-project` markers — a re-run regenerates what is inside them — and
  never let them bloat: once a detail stops being something you need on
  every turn, move it into the knowledge base and link it from here instead.
- Before changing the knowledge base, follow the `kb-maintenance.md` file in
  this project's knowledge base: it carries the format contract and the OKF
  spec-version check — never migrate silently and never ignore the drift.

บรรทัดด้านล่างคัดลอกมาจาก skill init-project แบบตรงตัวเป็นภาษาอังกฤษ ห้ามแก้ไขหรือแปล
<!-- karpathy:start -->
## Engineering guidelines (Karpathy)

Condensed from the [Karpathy guidelines](https://github.com/multica-ai/andrej-karpathy-skills) (MIT) — Andrej Karpathy's observations on LLM coding pitfalls, distilled into four principles:

1. **Think before coding.** Don't assume, don't hide confusion, surface tradeoffs — state assumptions explicitly, present alternatives instead of picking silently, and push back when a simpler approach exists.
2. **Simplicity first.** Minimum code that solves the problem, nothing speculative: no unrequested features, abstractions, or flexibility. If 200 lines could be 50, rewrite it.
3. **Surgical changes.** Touch only what you must; clean up only your own mess. Don't refactor or "improve" adjacent code — remove only the imports/variables your own change orphaned.
4. **Goal-driven execution.** Define verifiable success criteria and loop until met — e.g. "fix the bug" becomes "write a test that reproduces it, then make it pass."

Opt-out: delete this block, and answer "opt out" to the Karpathy question on the next init-project run — a re-run regenerates it while that answer is "include".
<!-- karpathy:end -->

## Agent notes

- **Claude Code:** import-adapter ผ่าน `CLAUDE.md`
- **Codex:** native — ห้ามรัน `/init` ที่นี่ เพราะจะสร้าง `AGENTS.md` ทับ
- **Cursor:** native — อ่าน `AGENTS.md` โดยตรง; ไม่มี `/init`
- **Gemini CLI:** import-adapter ผ่าน `GEMINI.md`
<!-- init-project:end -->
