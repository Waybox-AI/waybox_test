# waybox_test
wanna start ur career as EE??

# Waybox Hardware Design Exam
Overview
This assessment contains three questions that test your ability to review hardware projects, reason about power & display interfaces, and communicate your findings.
You will work on two existing projects:

File	Board nickname & Purpose (high‑level)
DOUBLE_CAMERA_SCARY.eprj	Board #1	Dual‑camera interface & processing
OMO ‑ WayBox.eprj	Board #2	Main control board (“WayBox”)

❓ Questions & Tasks
#	Task	Expected deliverables
1. Design review & fix	Open DOUBLE_CAMERA_SCARY.eprj.
• List every design flaw you spot (signal‑integrity, power, layout, footprints, net naming …)
• Fix the project (schematic or PCB) so it is production‑ready.
• Commit your patched .eprj (and any edited libs) under a folder fixed/board1/.	- fixed/board1/DOUBLE_CAMERA_SCARY.eprj
•A Markdown bullet list of each issue before / after in README.md
2. Power feasibility	Suppose you power Board #2 (OMO ‑ WayBox.eprj) board2 rail directly from a 3 .3 V MCU GPIO pin.
• Will Board #2 still be able to drive a 40‑pin RGB565 TFT‑LCD reliably?
• Explain why / why not (voltage levels, current capability, LCD back‑light, rise‑time, latch timings …)	- A paragraph in README.md
- Cite datasheet figures or equations where relevant
3. Functional summary	Write an engineer‑level overview of what each board does and how they interact. Focus on: key ICs, I/O headers, intended use‑cases, typical power budget.	- Section “Board summaries” in README.md (100 – 200 words per board)

🚀 Submission workflow
Fork via template

Click Use this template → choose Private.

Name the repo waybox‑exam‑<your‑GitHub‑ID>.

Add the examiner

Settings → Collaborators → invite CodingMcnugget with Write access.

Work

Create a feature branch answers/first_push (or any name you like).

Commit often with meaningful messages.

Delivery

Open a Pull Request into main titled “Exam submission – <your name>”.

Make sure README.md contains answers for Q1‑Q3.

Verify that fixed/board1/ holds your corrected project file(s).
