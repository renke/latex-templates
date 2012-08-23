TEX_FILE_NAME=presentation

all:
	rubber --pdf ${TEX_FILE_NAME}.tex

clean:
	rubber --pdf --gzip --clean ${TEX_FILE_NAME}.tex
	rm -rf ${TEX_FILE_NAME}.nav
	rm -rf ${TEX_FILE_NAME}.out
	rm -rf ${TEX_FILE_NAME}.snm
	rm -rf ${TEX_FILE_NAME}.synctex.gz
	
dist:
	rubber --pdf --gzip ${TEX_FILE_NAME}.tex

	
