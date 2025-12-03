# Curriculum Vitae - Christophe Trefois

A professional CV built with LaTeX using the ModernCV template, featuring automated builds and releases via GitHub Actions.

## 📄 Latest Version

Get the latest version of the CV in PDF format here: [Trefois CV PDF](https://github.com/Trefex/cv/releases/latest/download/Trefois_CV.pdf)

## 🛠️ Build

This repository uses GitHub Actions to automatically compile the LaTeX document into a PDF:

- **Release builds**: Triggered on version tags (e.g., `v1.0`), creating a GitHub release with the compiled PDF
- **Development builds**: Can be configured for testing changes

### Local Compilation

To compile the CV locally, you need a LaTeX distribution with `biblatex` and `biber` support:

```bash
pdflatex Trefois_CV.tex
biber Trefois_CV
pdflatex Trefois_CV.tex
pdflatex Trefois_CV.tex
```

Or use `latexmk` for automated compilation:

```bash
latexmk -pdf Trefois_CV.tex
```

## 📋 Features

- **Modern styling** using the ModernCV class with classic style and blue color scheme
- **Timeline visualization** with the `moderntimeline` package for experience chronology
- **Bibliography management** using BibLaTeX for publications
- **Professional sections**: Experience, Education, Skills, Languages, Publications, and more
- **Custom formatting** for dates, entries, and layout

## 📁 Repository Structure

```
.
├── .github/
│   └── workflows/          # GitHub Actions workflows
├── img/                    # Images (CV photo, etc.)
├── LICENSE                 # MIT License
├── publications.bib        # BibTeX bibliography file
├── README.md              # This file
└── Trefois_CV.tex         # Main LaTeX CV document
```

## 📦 Dependencies

The CV uses the following LaTeX packages:
- `moderncv` - CV template
- `moderntimeline` - Timeline visualization
- `biblatex` - Bibliography management
- `sourcesanspro` - Font
- `geometry` - Page layout
- `tikz/pgf` - Graphics and timeline rendering

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🔗 Links

- Personal website: [www.trefois.com](http://www.trefois.com)
- Publications: [www.trefois.com/home/publications](http://www.trefois.com/home/publications)
- LinkedIn: [trefoischristophe](https://linkedin.com/in/trefoischristophe)
- GitHub: [Trefex](https://github.com/Trefex)

