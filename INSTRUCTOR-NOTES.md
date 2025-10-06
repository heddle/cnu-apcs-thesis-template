# 🧑‍🏫 CNU APCS Thesis Template – Instructor Update Checklist

This checklist is for maintainers (faculty) to update the template if the **CNU Thesis Style Manual** is revised.  

---

## 📂 Files to Review/Update
- **cnu-thesis.sty**
  - Margins (geometry package)
  - Fonts (Times New Roman requirement)
  - Spacing (double vs single in special cases)
  - Page numbering (Roman vs Arabic)
  - Commands to check:
    - \apcsabstract (abstract format)
    - \thesistitlepage (committee signature lines)
    - \dedication, \acknowledgements
    - \literaturecited
    - \cnuTable, \cnuFigure

- **thesis.tex**
  - Student placeholders, ensure they reflect current manual.

- **thesis-sample.tex**
  - Demonstrates formatting: title page, abstract, chapters, table, figure, references.
  - Fake committee names should look realistic and follow current style manual.

- **README.md**
  - Instructions for students.
  - Ensure usage examples match macro definitions.

- **references.bib**
  - Sample entries should match required citation style if updated.

---

## 🔎 Formatting Points to Verify Each Year
- Font family and size
- Margins (left, right, top, bottom)
- Abstract rules (word count, no equations/figures)
- Signature page wording (committee labels, signature lines)
- Spacing rules (double spacing, single-spaced references)
- Page order (Abstract → Title Page → Dedication → Acknowledgements → TOC → Lists → Chapters → References → Appendices → Blank page)
- Caption placement (tables above, figures below)
- Page numbering conventions (Roman vs Arabic)

---

## ⚙️ Overleaf/GitHub Maintenance
- If changes are made:
  1. Update `cnu-thesis.sty`.
  2. Update `thesis-sample.tex` to reflect new formatting.
  3. Update `README.md` for students.
  4. Update version/date in README.
  5. Commit and push changes to GitHub.
  6. Create a new GitHub Release (e.g., v1.1).

---

## 📝 Faculty Notes
- Keep this file **out of student-facing docs** (not referenced in README).
- This is for internal instructor use only.
