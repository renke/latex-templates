TEX_FILE_NAME=presentation

all: clean
	pdflatex ${TEX_FILE_NAME}.tex
	bibtex -terse ${TEX_FILE_NAME}.aux || true
	pdflatex ${TEX_FILE_NAME}.tex
	pdflatex -synctex=1 ${TEX_FILE_NAME}.tex

clean:
	rm -rf ${TEX_FILE_NAME}.aux
	rm -rf ${TEX_FILE_NAME}.bbl
	rm -rf ${TEX_FILE_NAME}.blg
	rm -rf ${TEX_FILE_NAME}.idx
	rm -rf ${TEX_FILE_NAME}.ilg
	rm -rf ${TEX_FILE_NAME}.ind
	rm -rf ${TEX_FILE_NAME}.log
	rm -rf ${TEX_FILE_NAME}.nav
	rm -rf ${TEX_FILE_NAME}.out
	rm -rf ${TEX_FILE_NAME}.pdf
	rm -rf ${TEX_FILE_NAME}.snm
	rm -rf ${TEX_FILE_NAME}.synctex.gz
	rm -rf ${TEX_FILE_NAME}.toc
	
