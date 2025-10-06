# 📘 CNU APCS Thesis Template (LaTeX, Overleaf & GitHub)

This repository provides a LaTeX thesis template for the **Master of Science in Applied Physics and Computer Science (APCS)** program at **Christopher Newport University (CNU)**.

It follows the **2019 CNU Thesis Style Manual** requirements for APCS formatting.

## 📂 What’s Included
- `thesis.tex` — main student file  
- `cnu-thesis.sty` — style file enforcing thesis rules  
- `references.bib` — example bibliography file  
- `example-image.png` — placeholder figure  
- `README.md` — instructions  

## 🚀 How to Use

### Overleaf (Recommended)
1. Download this repo as a ZIP (`Code → Download ZIP`)  
2. Go to [Overleaf](https://overleaf.com)  
3. New Project → Upload Project → Upload ZIP  

### Local TeX
Compile with:
```bash
latexmk -pdf -bibtex thesis.tex
```

## ✍️ Usage Examples
Abstract:
```latex
\apcsabstract{Title}{Student Name}{2025}{Advisor}{Abstract text}
```

Citing references:
```latex
As shown in \cite{einstein1905}, ...
```

Table:
```latex
\cnuTable{Caption}{\begin{tabular}{|c|c|}\hline A & B \\\hline 1 & 2 \\\hline\end{tabular}}
```

Figure:
```latex
\cnuFigure{Caption}{\includegraphics[width=0.6\textwidth]{example-image}}
```

## 📝 Notes
- Abstract ≤150 words, double-spaced  
- Chapter headings ALL CAPS, bold, centered  
- No running headers  
- Submit single-sided PDF with required blank pages  

Maintainer: **[Your Name / Department Contact]**  
Version: **October 2025**
