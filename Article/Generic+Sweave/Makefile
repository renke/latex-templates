SWEAVE_FILE_NAME=article
TEX_FILE_NAME=article
#R_FILE_NAME=article

all:
	R CMD Sweave ${SWEAVE_FILE_NAME}.Rnw
	pdflatex ${TEX_FILE_NAME}.tex
	bibtex ${TEX_FILE_NAME}.aux
	pdflatex ${TEX_FILE_NAME}.tex
	pdflatex -synctex=1 ${TEX_FILE_NAME}.tex

clean:
	rm -rf ${TEX_FILE_NAME}-sweave-fig-*.pdf
	rm -rf ${TEX_FILE_NAME}.aux
	rm -rf ${TEX_FILE_NAME}.bbl
	rm -rf ${TEX_FILE_NAME}.blg
	rm -rf ${TEX_FILE_NAME}.idx
	rm -rf ${TEX_FILE_NAME}.ilg
	rm -rf ${TEX_FILE_NAME}.ind
	rm -rf ${TEX_FILE_NAME}.log
	rm -rf ${TEX_FILE_NAME}.out
	rm -rf ${TEX_FILE_NAME}.pdf
	rm -rf ${TEX_FILE_NAME}.synctex.gz
	rm -rf ${TEX_FILE_NAME}.tex
	rm -rf texput.log
#	rm -rf ${R_FILE_NAME}.R
	
