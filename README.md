# 📘 CNU APCS Thesis Template (LaTeX, Overleaf & GitHub)

This repository provides a LaTeX thesis template for the **Master of Science in Applied Physics and Computer Science (APCS)** program at **Christopher Newport University (CNU)**.

It follows the **2019 CNU Thesis Style Manual** requirements for APCS formatting.

---

## 📂 What’s Included
- `thesis.tex` — **blank starter file** with placeholders (for students to fill in)  
- `thesis-sample.tex` — **pre-filled demo thesis** (Jane Doe, with example chapters, table, figure, references, committee page)  
- `cnu-thesis.sty` — style file enforcing thesis rules  
- `references.bib` — example bibliography file (with Einstein, Maxwell, Feynman)  
- `example-image.png` — placeholder figure  
- `README.md` — this guide  

---

## 🚀 How to Use

### Option 1: Overleaf (Recommended)
1. Download this repo as a ZIP (`Code → Download ZIP`)  
2. Go to [Overleaf](https://overleaf.com)  
3. New Project → Upload Project → Upload ZIP  

- Edit `thesis.tex` for your own thesis.  
- If you want to see how a completed thesis looks, open and compile `thesis-sample.tex`.  

### Option 2: Local TeX
Compile with:
```bash
latexmk -pdf -bibtex thesis.tex
```
(Use `biber` if running with BibLaTeX backend.)

---

## ✍️ Usage Examples

### Abstract
```latex
pcsabstract
{THESIS TITLE}
{STUDENT NAME}
{2025}
{ADVISOR NAME, DEGREE, TITLE, DEPARTMENT}
{ABSTRACT TEXT (≤150 words).}
```

### Title Page with Committee
The command `\thesistitlepage` now takes **6 arguments**:

```latex
	hesistitlepage
{THESIS TITLE}           % 1. Title
{STUDENT NAME}           % 2. Author
{YEAR}                   % 3. Year
{COMMITTEE MEMBER 1}     % 4. Chair
{COMMITTEE MEMBER 2}     % 5. Member
{COMMITTEE MEMBER 3}     % 6. Member
```

Example:
```latex
	hesistitlepage
{A STUDY OF SIMULATED WIND TUNNEL DATA}
{JANE DOE}
{2025}
{PROF. SAM SMITH}
{DR. LINDA JONES}
{DR. ROBERT TAYLOR}
```

This produces the author’s name at the top, the standard submission wording, and three aligned signature lines for approval.

### Citations
Add references to `references.bib`:
```bibtex
@article{einstein1905,
  author  = {Albert Einstein},
  title   = {Does the Inertia of a Body Depend Upon Its Energy Content?},
  journal = {Annalen der Physik},
  year    = {1905},
  volume  = {18},
  pages   = {639--641}
}
```
Then cite in text:
```latex
As shown in \cite{einstein1905}, energy and mass are equivalent.
```

### Tables
```latex
\cnuTable{Experimental Results}{
egin{tabular}{|c|c|}
\hline
A & B \\
\hline
1 & 2 \\
\hline
\end{tabular}
}
```

### Figures
```latex
\cnuFigure{Sample Plot}{
\includegraphics[width=0.6	extwidth]{example-image}
}
```

---

## 📝 Notes
- Abstract ≤150 words, no formulas/diagrams.  
- Chapter headings ALL CAPS, bold, centered.  
- No running headers.  
- Submit single-sided PDF with required blank pages.  
- Use `thesis.tex` for your actual thesis.  
- `thesis-sample.tex` is only a **demo** to show correct formatting (including committee signature page).  

---

## 🎓 Maintainer
Maintainer: **David Heddle**  
Professor of Physics, Christopher Newport University  
📧 david.heddle@cnu.edu  
Version: **October 2025**
