# Syllabuild

<img width="859" height="588" alt="image" src="https://github.com/user-attachments/assets/ada0c305-12f1-4688-ab67-82550c167c2a" />

**[Try it live](https://digitaldickinson.github.io/syllabuild/syllabuild.html)** — no download or install required.

A local-first, zero-dependency, single-file curriculum design application tailored for UK Higher Education modules. 

Syllabuild bridges the gap between pedagogical software planning and rigid academic administrative compliance. It allows unit leaders to construct rich linear schedules, calculate notional student workloads, map curriculum requirements, and export clean snippets directly to Virtual Learning Environments (VLEs) or validation documents.

---

## Key Features

### 1. Dynamic Workload Analytics
* **Automated Hour Calculations:** Instantly tracks total contact hours against credit sizing metrics (1 credit = 10 notional learning hours) in a sticky dashboard.
* **Independent Study Guidance:** Automatically generates suggested independent study targets based on class contact times.

### 2. Built for VLE & Validation Workflows
* **Granular VLE Export:** Clean, inline-sanitized HTML snippets produced specifically for Moodle or alternative platform text areas.
* **Document Synchronization:** Visual "Export Drift" indicators highlight if content has been modified since it was last copied to external platforms.
* **Macro Exports:** Generates fully stylized `.docx` files for formal curriculum validation processes and `.ics` calendar files with one event per confirmed Contact Day.
* **Per-Week Contact Days:** Mon–Fri checkboxes on each week card, each showing its actual calendar date, so class weeks can be marked independently (e.g. for reading weeks or bank holidays).

### 3. Native Policy & Evidence Mapping
* **Curriculum Checklists:** Explicit fields to track Work Informed Learning (**WIL**) and Education for Sustainable Development (**ESD**) indicators.
* **Compliance Flags:** Dedicated tracking for institutional reviews (e.g., DELTA and RIPIAG frameworks).
* **Automated Appendix Generation:** Toggled framework checkmarks automatically build organized pedagogical evidence sections inside formal document exports.

### 4. Lightweight & Secure
* **Local-First State:** Full module configurations save down to a portable, lightweight `.syllabuild` JSON format.
* **Accidental-Close Protection:** Warns before an accidental back button or tab close if there are unsaved changes, and silently drafts your in-progress work to the browser so it can be recovered after a crash.
* **Keyboard & Screen Reader Accessible:** Dialogs and panels follow standard WAI-ARIA patterns (focus trapping and restoration in modals, `aria-expanded`/`inert` disclosure for the Configure panel, full Escape-key support).
* **Zero Infrastructure Requirements:** Written in vanilla JavaScript with an architecture requiring no Node engine runtime, external databases, or server configurations.

### 5. Multiple Planning Views
* **Cards / Timeline / Status Board:** Switch the week strip between a card-per-week view, a row-based timeline showing Contact Days and assessment markers across every week at a glance, and a status board that groups weeks by readiness (Pending / Partial / Completed / External Factor).

---

## Technical Stack

* **Core Language:** Native Vanilla HTML5 / ES6 JavaScript / CSS3 Variables.
* **Rich Text Editing:** Quill.js WYSIWYG editor engine (tailored run context with filtered asset sanitization allowlists).
* **Document Processing:** html-docx-js / FileSaver.js for client-side blob generation.

---

## Getting Started

1. Use the [hosted version](https://digitaldickinson.github.io/syllabuild/syllabuild.html) directly in your browser, or download/clone the `syllabuild.html` source file and double-click it to launch it natively inside any contemporary modern web browser.
2. Open the **Configure** drawer to set structural metadata (such as credits, target terms, or weekly teaching contact allocation).
3. Save your progress down locally as a `.syllabuild` backup asset at any point using the top-level control panel.

---

## Development Notes

Parts of this application were developed with the assistance of AI coding agents.
