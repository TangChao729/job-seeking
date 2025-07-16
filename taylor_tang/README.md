# Taylor Tang - CV & Resume

This directory contains Taylor Tang's personal CV, resume, and cover letter templates built with Awesome CV.

## Structure

```
taylor_tang/
├── README.md           # This file
├── Makefile           # Build automation
├── awesome-cv.cls     # LaTeX class file
├── resume.tex         # Resume template
├── cv.tex             # CV template  
├── coverletter.tex    # Cover letter template
├── sections/          # Individual content sections
│   ├── summary.tex
│   ├── experience.tex
│   ├── project.tex
│   ├── education.tex
│   ├── honors.tex
│   └── certificates.tex
└── images/            # Profile images and assets
    └── ghibli_studio_2.png
```

## Building Documents

### Prerequisites
- XeLaTeX (part of TeX Live distribution)
- Make (optional, for using Makefile)

### Quick Start

Build all documents:
```bash
make all
```

Build individual documents:
```bash
make resume      # Builds resume.pdf
make cv          # Builds cv.pdf  
make coverletter # Builds coverletter.pdf
```

Manual compilation:
```bash
xelatex resume.tex
xelatex cv.tex
xelatex coverletter.tex
```

Clean generated files:
```bash
make clean
```

## Customization

### Personal Information
Update your contact details in each main `.tex` file:
- `resume.tex`
- `cv.tex` 
- `coverletter.tex`

### Content Sections
Edit the files in the `sections/` directory:
- `summary.tex` - Professional summary
- `experience.tex` - Work experience
- `project.tex` - Project highlights
- `education.tex` - Educational background
- `honors.tex` - Awards and achievements
- `certificates.tex` - Certifications

### Colors and Styling
Change the color scheme in any main `.tex` file:
```latex
\colorlet{awesome}{awesome-red}
% Available: awesome-emerald, awesome-skyblue, awesome-red, 
%           awesome-pink, awesome-orange, awesome-nephritis, 
%           awesome-concrete, awesome-darknight
```

### Customization for Job Applications
1. **Resume**: Edit sections in `sections/` directory to emphasize relevant skills
2. **Cover Letter**: Update recipient info, position title, and customize content
3. **Colors**: Change theme colors to match company branding if desired

## Output
Generated PDF files will be created in this directory:
- `resume.pdf`
- `cv.pdf`
- `coverletter.pdf` 