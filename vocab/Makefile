all: ./vocabs.pdf #10.pdf #12.pdf #11.pdf 09.pdf | build

build:
	-mkdir build

%.pdf: %.tex
	latexmk -dvi- -pdf -interaction=nonstopmode -file-line-error -output-directory=build $<

clean:
	latexmk -C -output-directory=build
