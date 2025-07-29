# Waybox Hardware Design Exam 🛠️

Welcome!  
This take‑home test assesses your ability to **review hardware projects, reason about power & display interfaces, and communicate clearly**.  
You will work with two existing Altium/Protel projects:

| File | Board nickname | High‑level purpose |
|------|----------------|--------------------|
| `DOUBLE_CAMERA_SCARY.eprj` | **Board #1** | Dual‑camera interface & processing |
| `OMO ‑ WayBox.eprj`       | **Board #2** | Main control board (“WayBox”) |

---

## 📋 Questions & Deliverables

| # | Task | What you must submit |
|---|------|---------------------|
| **1 – Design review & fix** | *Open* **`DOUBLE_CAMERA_SCARY.eprj`**.<br>1. List **every design flaw** you identify (signal‑integrity, power, layout, footprints, net naming, etc.).<br>2. **Fix the project** (schematic and/or PCB) so it is production‑ready.<br>3. Place the corrected files in `fixed/board1/`. | - `fixed/board1/DOUBLE_CAMERA_SCARY.eprj` (+ any edited libraries)<br>- A bullet list of each issue **before / after** in `README.md` |
| **2 – Power feasibility** | Suppose **Board #2** is powered only by a **3 .3 V MCU GPIO pin** on *board2* rail.<br>- Can Board #2 still **drive a 40‑pin RGB565 TFT‑LCD** reliably?<br>- *Why or why not?* (consider voltage levels, current, back‑light, rise‑time, latch timing, etc.) | A ±150‑word explanation in `README.md`, citing datasheet numbers or equations. |
| **3 – Functional summary** | Provide an engineer‑level summary of **what each board does** and how they interact. Mention key ICs, I/O headers, intended use‑cases, typical power budget. | Section **“Board summaries”** in `README.md` (≈ 100–200 words per board). |

---

## 🚀 Submission Workflow

1. **Create your private repo**  
   1. Click **“Use this template”** (top‑right).  
   2. **Visibility → Private**.  
   3. Name it `waybox‑exam‑<your‑github‑id>`.

2. **Invite the examiner**  
   - Settings → Collaborators → **add `CodingMcnugget`** with *Write* access.

3. **Work**  
   ```bash
   # example local setup
   git clone git@github.com:<you>/waybox-exam-<id>.git
   git checkout -b answers/first_push
