filename = rapport_son
variable = $(filename).tex

all: pdflatex

pdflatex: $(variable)
	pdflatex $(variable)
	bibtex $(filename)
	pdflatex $(variable)
	pdflatex $(variable)

clean:
	rm $(filename).aux $(filename).pdf $(filename).glo $(filename).gls $(filename).bbl $(filename).log $(filename).blg $(filename).dvi $(filename).out

show: pdflatex
	evince $(filename).pdf

