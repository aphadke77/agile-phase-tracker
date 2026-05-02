# Agile Phase Tracker

A lightweight, single-file dashboard for tracking progress across all phases of an Agile project lifecycle — no backend, no install, no dependencies.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML](https://img.shields.io/badge/built%20with-HTML%2FJS-orange.svg)
![No dependencies](https://img.shields.io/badge/dependencies-none-brightgreen.svg)

---

## Features

- **Multi-project tracking** — manage any number of projects from one dashboard
- **12 Agile phases** — follows an improved, validated Agile delivery flow
- **Per-phase status** — set each phase to `Pending`, `Active`, `Done`, or `Blocked`
- **Sprint assignment** — tag each phase with its sprint number
- **Project status cycling** — click the status badge to rotate through `Planning → Active → On Hold → Complete`
- **Progress visualization** — colour-coded mini bar and percentage per project
- **Live stats bar** — total projects, active count, average progress, and blocked phase count
- **Filter & search** — filter by project status or search by name/code
- **Notes per project** — free-text field for impediments, decisions, and sprint context
- **Export to JSON** — download all projects or a single project as a dated JSON file
- **Restore from JSON** — import with three modes: Merge, Replace matching, or Overwrite all
- **Persistent storage** — data saved to browser `localStorage`; survives page refresh

---

## The 12 Agile Phases

| # | Phase |
|---|-------|
| 1 | Discover & Define User Stories |
| 2 | Backlog Grooming & Refinement |
| 3 | Effort Estimation |
| 4 | Build Product Backlog |
| 5 | Prioritize Backlog |
| 6 | Sprint Planning |
| 7 | Resource Allocation |
| 8 | Sprint Execution |
| 9 | Track Sprint Progress |
| 10 | Sprint Review / Demo |
| 11 | Sprint Retrospective |
| 12 | Release & Deploy |

> **Note:** Phase 2 (Backlog Grooming) is a recurring mid-sprint ceremony — it can be marked Active in parallel with Sprint Execution. A **Blocked** status indicates an impediment that must be resolved before that phase can proceed.

---

## Getting Started

### Option 1 — Use directly in browser

1. Download `index.html`
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari)
3. Start adding projects — no setup required

### Option 2 — GitHub Pages (live URL)

1. Fork or clone this repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your tracker will be live at `https://yourusername.github.io/agile-phase-tracker`

---

## Usage

### Adding a project
Click **+ NEW PROJECT** in the top-right corner and fill in the project name, code, status, sprint range, and owner.

### Tracking phases
Expand a project card to see all 12 phases. Use the dropdown on each phase cell to update its status, and enter the sprint number it belongs to.

### Changing project status
Click the coloured status badge (`Planning`, `Active`, `On Hold`, `Complete`) on any project card to cycle through statuses.

### Exporting data
Click **⬇ Data** in the header to open the Data panel. Export all projects or a single project as a JSON file.

### Restoring data
In the Data panel, drag and drop (or browse for) a previously exported `.json` file. Choose a restore mode before confirming:

| Mode | Behaviour |
|------|-----------|
| **Merge** | Adds new projects only; skips projects that already exist (safe default) |
| **Replace matching** | Adds new projects and overwrites existing ones by ID |
| **Overwrite all** | Replaces all current data with the imported file |

---

## Data & Privacy

- All data is stored in your **browser's `localStorage`** — nothing is sent to any server
- Clearing browser data or using a different browser will result in a fresh tracker
- Use the **Export** feature regularly to back up your data as JSON files
- Exported JSON files can be version-controlled in this repository alongside the tracker

---

## Browser Support

Works in all modern browsers. No server, framework, or build step required.

| Browser | Supported |
|---------|-----------|
| Chrome 90+ | ✅ |
| Firefox 88+ | ✅ |
| Edge 90+ | ✅ |
| Safari 14+ | ✅ |

---

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

---

## License

MIT — see [LICENSE](./LICENSE) for details.
