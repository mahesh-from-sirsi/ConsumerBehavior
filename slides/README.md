# Consumer Behaviour lecture slides — browser presentation assets

These slides are referenced by **[Lecture Presentations](../slides.html)** and integrated into the main [Learning Hub](../index.html).

| Module | Presentation | Pages displayed | Source |
|---|---|---:|---|
| 1 | Introduction to Consumer Behaviour | 148 | Faculty-supplied PowerPoint |
| 2 | Consumer Decision Making | 84 | Faculty-supplied PowerPoint |
| 3 | Individual Determinants of Consumer Behaviour | 89 | Faculty-supplied PowerPoint |
| 4 | Group Determinants of Consumer Behaviour | 79 | Faculty-supplied PowerPoint |
| 5 | Environmental Influences | Pending | Faculty will supply later |
| 6 | Customer Relationship Management | Pending | Faculty will supply later |

## How it works

- `viewer.html?module=1` reads `data/module-1.pdf` directly.
- For Modules 2–4, GitHub stores each PDF's base64 in consecutive `data/module-N-XX.b64` UTF-8 text assets. The viewer downloads them, decodes each chunk, and reconstructs a PDF in browser memory for the built-in PDF viewer. This avoids per-request size limits when uploading through the connected GitHub integration. It is not a transcription or a new slide deck: the resulting PDF bytes were verified to exactly match the PowerPoint-to-PDF export.
- The source PowerPoint files remain unchanged and are **not** included in this repository. Students can download the PDF.
- Transitions, animations and embedded videos from PowerPoint are not supported in the PDF export.
- Module 3 has **95 slides in the original .pptx**; slides **37, 43, 44, 45, 46, 47** are marked *hidden* in the original deck, so the PDF/browser presentation includes **89 visible slides**.

## Adding Modules 5 and 6 later

Supply the PowerPoint deck and convert it to a browser PDF. Add the PDF to `data/` (or store it as ordered, independently base64-decodable text parts when the connection's size limit requires chunking), update `catalog` in `viewer.html`, enable the appropriate card in `../slides.html`, and update the existing module's homepage list entry. **Do not remove or overwrite the module's interactive lessons, notes, cases or quizzes.**

## Viewing limitations

The embedded PDF viewer depends on browser PDF support. Use the **Download PDF** option if an embedded view is unavailable. Some browsers may ignore programmatic slide navigation; their native PDF toolbar should still work.
