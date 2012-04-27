TEX_FILE_NAME=article

all:
	rubber --pdf ${TEX_FILE_NAME}.tex

clean:
	rubber --pdf --clean ${TEX_FILE_NAME}.tex
	rm -rf ${TEX_FILE_NAME}.synctex.gz
	
dist:
	rubber --pdf --gzip ${TEX_FILE_NAME}.tex
