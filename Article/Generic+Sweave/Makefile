SWEAVE_FILE_NAME=article
TEX_FILE_NAME=article
#R_FILE_NAME=article

all:
	R CMD Sweave ${SWEAVE_FILE_NAME}.Rnw
	rubber --pdf ${TEX_FILE_NAME}.tex

clean:
	rubber --pdf --clean ${TEX_FILE_NAME}.tex
	rm -rf ${TEX_FILE_NAME}-sweave-fig-*.pdf
	rm -rf ${TEX_FILE_NAME}.synctex.gz
	rm -rf ${TEX_FILE_NAME}.tex

dist:
	rubber --pdf --gzip ${TEX_FILE_NAME}.tex
