# Signals and Systems — Project Phase 2: Sheet Music to Audio

Phase 2 of the **Signals and Systems** course project (Sharif University of Technology, Spring 2023), with Yahya Tehrani: a program that **reads a sheet-music image and plays it**.

## How it works

1. **Note detection** — finds note symbols on each staff line of the score with template matching (`cv2.matchTemplate`).
2. **Pitch and duration** — maps each note's position to its pitch (frequencies built from A0 = 27.5 Hz in 12-tone equal temperament) and its symbol to a duration based on the tempo (BPM).
3. **Synthesis** — generates the tone for each note and joins them into a single audio track.

Tested on *Twinkle, Twinkle, Little Star*, *Ave Maria*, *Polyushka-polye* and *Jane Maryam*.

## Contents

| File / folder | Description |
|---|---|
| `Phase2_signal_system.ipynb`, `Phase2_signal_system_2.ipynb` | Main implementation |
| [`SS-Project-Phase2/`](SS-Project-Phase2) | Assignment description, helper notebook, note templates, input scores and the LaTeX report (`main.pdf`) |
| `report.docx` | Report (Word version) |
| `SS-Project-Phase2_*.zip` | Submitted versions of the project |

## Tools

Python · OpenCV · NumPy · SciPy
