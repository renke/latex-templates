SWEAVE_FILE_NAME=article
TEX_FILE_NAME=article
#R_FILE_NAME=article

all:
	R -q -e "require('knitr'); knit('${SWEAVE_FILE_NAME}.Rnw')"
	rubber --pdf ${TEX_FILE_NAME}.tex
	rm NA

clean:
	rubber --pdf --gzip --clean ${TEX_FILE_NAME}.tex
	rm -rf ${TEX_FILE_NAME}-knitr-fig-*.pdf
	rm -rf ${TEX_FILE_NAME}.synctex.gz
	rm -rf ${TEX_FILE_NAME}.tex
	rm -rf NA
	rm -rf auto
	rm -rf cache
dist:
	rubber --pdf --gzip ${TEX_FILE_NAME}.tex
