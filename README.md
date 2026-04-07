# THD-Campus-Cham-Thesis-LATEX-Template

This repository provides an **unofficial LaTeX setup** for academic theses intended for use at the **Deggendorf Institute of Technology (THD), Cham Campus**.

It is suitable for **Master thesis** and uses a **deterministic, examiner-safe build process** based on **XeLaTeX** and **BibTeX**.

> ⚠️ **Disclaimer**  
> This is **not an official THD Campus Cham Thesis template**.  
> Students are responsible for ensuring that the final document complies with the **latest THD thesis submission guidelines**.

## Cloning the Repository

Clone the repository using Git:

```bash
git clone https://github.com/IndominusPsych/THD-Campus-Cham-Thesis-LATEX-Template.git
```

## Prerequisites

### LaTeX Distribution

A LaTeX distribution with **XeLaTeX** and **BibTeX** support is required.

- **Windows:** MiKTeX
- **macOS:** MacTeX
- **Linux:** TeX Live

Verify the installation:

```bash
xelatex --version
bibtex --version
```

## Build Tools

### Required Tools

- `make`
- `bibtex`

On **Windows**, the following may also be required:

- Strawberry Perl
- GNU Make (via **MSYS2**, **Chocolatey**, or **WSL**)
- Git
- VS Code
- Latex Workshop (VS Code Extension)

Verify Git installation:

```bash
git --version
```

## Build Configuration

XeLaTeX is executed in the following order using LaTeX Workshop extension.

```
XeLaTeX → BibTeX → XeLaTeX → XeLaTeX
```

This ensures that the following are fully resolved:

- References
- Cross-references
- Table of contents

The output file `thesis.pdf` is generated in the same directory as `thesis.tex`.

## License

This project is licensed under the **MIT License**.  
See the `LICENSE` file for details.
