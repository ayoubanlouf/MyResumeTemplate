# LaTeX Resume Template

A clean, modern, ATS-friendly **LaTeX résumé/CV template** designed for software engineers, DevOps practitioners, and tech professionals. 

Everything is self-contained in a single, customizable file: [`template.tex`](./template.tex).

---

## 📂 Structure

- **`template.tex`** → Self-contained resume template containing layout styling, macros, personal information, education, experience, projects, and skills.

---

## ✏️ How to Customize

Open `template.tex` and modify the relevant sections:

### 1. Personal Information & Header
Update the contact definition block:
```latex
\def\firstname{Firstname}
\def\lastname{Lastname}
\def\email{firstname.lastname@example.com}
\def\linkedin{https://linkedin.com/in/username}
\def\github{https://github.com/username}
\def\jasphone{+1 (555) 000-0000}
```

### 2. Education
Define your degree and institution:
```latex
\EducationTemplate{College}{StartYear}{EndYear}{University / College Name}{Degree Title}{}
```

### 3. Experience & Internships
Add work experience using `StageTemplate`:
```latex
\StageTemplate{id}{Date Range}{Key Technologies}{Role / Designation}{Company Name (Location)}{
  \jbegin
    \jitem{Key achievement or contribution with metrics}
    \jitem{Action-oriented bullet point describing technical impact}
  \jend
}
```
Render it in the document body:
```latex
\renderExp{id}
```

### 4. Projects
Add projects using `ExpTemplate`:
```latex
\ExpTemplate{id}{Technologies Used}{Project Title}{Date}{
  \jbegin
    \jitem{Overview of technical implementation and architecture}
    \jitem{Quantifiable performance improvement or key capability}
  \jend
}
```
Render it in the document body:
```latex
\renderExp{id}
```

### 5. Technical Skills & Certifications
- Edit `\achievements` to categorize your technical competencies (Languages, Cloud/DevOps, Frameworks, Tools).
- Edit `\certifications` to list your verified credentials.

---

## ⚙️ Compilation

### Local Compilation (PDFLaTeX)
```bash
pdflatex template.tex
```

### Local Compilation (Tectonic)
```bash
tectonic template.tex
```

### Overleaf
Upload `template.tex` directly into Overleaf with `pdfLaTeX` or `XeLaTeX` compiler.
