.PHONY: all resume cv coverletter clean test

CC = xelatex

# Build all documents
all: resume cv coverletter

# Individual targets
resume: resume.pdf
cv: cv.pdf
coverletter: coverletter.pdf

# Build rules
resume.pdf: resume.tex sections/*.tex
	$(CC) resume.tex

cv.pdf: cv.tex sections/*.tex
	$(CC) cv.tex

coverletter.pdf: coverletter.tex
	$(CC) coverletter.tex

# Test build (quick compilation check)
test:
	$(CC) --interaction=nonstopmode resume.tex > /dev/null 2>&1 && echo "✓ Build test passed" || echo "✗ Build test failed"

clean:
	rm -f *.pdf *.aux *.log *.out *.fdb_latexmk *.fls *.synctex.gz 