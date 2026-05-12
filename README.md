# LaTeX Resume Template

This repository contains a **LaTeX résumé/CV template** designed for clarity, ATS‑compatibility, and easy customization.  
It is inspired by **Jaskirat Singh**’s Overleaf résumé template, adapted and simplified for personal use.

---

## 📂 Structure

- `main.tex` → Controls layout, sections, and formatting.  
- `particulars.tex` → Contains all personal data, education, projects, experiences, skills, and certifications.  
- `utilities.tex` → Defines macros (`EducationTemplate`, `ExpTemplate`, etc.) used to structure entries.  

---

## ✏️ How to Edit

- **Personal info** → Found in `particulars.tex` (`firstname`, `lastname`, `email`, `linkedin`, `github`, `jasphone`).  
- **Education** → Add or edit entries using `EducationTemplate` in `particulars.tex`.  
- **Projects** → Add or edit entries using `ExpTemplate` in `particulars.tex`.  
- **Experience/Internships** → Add or edit entries using `StageTemplate` in `particulars.tex`.  
- **Hackathons/Other activities** → Add or edit entries using `HckTemplate` in `particulars.tex`.  
- **Skills & Certifications** → Defined in `achievements` and `certifications` blocks in `particulars.tex`.  

---

## ⚙️ Compilation

To generate the PDF résumé, run:

```bash
pdflatex main.tex
```

This will produce main.pdf with your customized résumé.
