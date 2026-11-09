# Paper

LaTeX write-up of the Society-5 project:

> **Robosapien – model of AI traveler**
> *Towards Future Society 5.0: Modeling, Exploration & Understanding*
>
> Alex Tsvetanov (Sofia High School of Mathematics) & Ivaylo Ivanov (High School of Natural Sciences and Mathematics, Stara Zagora)
> Under the direction of Assoc. Prof. Zlatogor Minchev
> Summer Research School (SRS) of the High School Students Institute of Mathematics and Informatics, Pamporovo, Bulgaria, August 2018

📄 **[documentation.pdf](./documentation.pdf)** is the last compiled version (11 Aug 2018).

## Abstract (summary)

The project shows a WowWee Robosapien X working as a "robo-researcher". It explores an environment and avoids obstacles without a human controlling it, as a stand-in for a planetary-exploration mission such as one on Mars. A mixed-reality interface also lets a person see through the robot's camera and control it remotely.

## Structure

| File | Section |
|---|---|
| `documentation.tex` | Main document: title page, abstract, bibliography. Includes the sections below with `subfiles` |
| `introduction.tex` | Introduction: AI, VR and humanoid robots as building blocks of Society 5.0 |
| `implementation.tex` | Hardware, software, algorithms and communication: QR-code recognition, computer vision, infrared control, VR control |
| `techniques.tex` | Tools: C# sender for IR commands recorded from the original remote |
| `problems.tex`, `future.tex` | Unfinished (TODO). Future-work notes list a 360° camera, arm control and better mechanics |
| `project.bib` | Bibliography stub |
| `robot.png` | Title-page photo of the robot |

## Build

```bash
pdflatex documentation.tex
```

## Notes

- The text calls Robosapien "NASA's prototype robot". In fact Robosapien is a WowWee toy designed by Mark Tilden, a robotics physicist known for his earlier work at Los Alamos National Laboratory; it was not a NASA prototype. The original 2018 text is kept unchanged here.
- The sources were deleted from this repository by commit `15d3230` ("filter and re-order") and later restored from `ef60b8f`.
- `Intro.pdf` in the [Introduction](https://github.com/Society-5/Introduction) repository is an earlier draft of this paper's abstract (10 Aug 2018).
- Related earlier work by the same group: Z. Minchev, L. Boyanov, A. Georgiev, A. Tsvetanov, *An Analytical Outlook towards Digital Training Security Transformations*, ICAICTSEE-2017, UNWE, Sofia (VR "virtual teacher" and mixed-reality training layers).

---

Part of **[Society-5](https://github.com/Society-5)**: a WowWee Robosapien X that explores a floor on its own, using a phone camera and QR codes as markers, with a mixed-reality (VR) interface for remote control.
