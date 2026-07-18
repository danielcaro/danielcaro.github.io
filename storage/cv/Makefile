PDFLATEX = /usr/bin/pdflatex
FLAGS = -file-line-error -interaction=nonstopmode -synctex=1 -output-format=pdf -output-directory=./out

SPANISH_TEX = CV_Spanish.tex
ENGLISH_TEX = CV_English.tex

SPANISH_PDF = ./CV_Spanish.pdf
ENGLISH_PDF = ./CV_English.pdf

all: $(SPANISH_PDF) $(ENGLISH_PDF)

$(SPANISH_PDF): $(SPANISH_TEX)
	$(PDFLATEX) $(FLAGS) $(SPANISH_TEX)

$(ENGLISH_PDF): $(ENGLISH_TEX)
	$(PDFLATEX) $(FLAGS) $(ENGLISH_TEX)

clean:
	rm -rf ./out/*

.PHONY: all clean
