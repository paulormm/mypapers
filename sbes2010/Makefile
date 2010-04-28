TARGET=sourcecode_attractiveness

all: $(TARGET).pdf
	evince $(TARGET).pdf &

$(TARGET).pdf: $(TARGET).tex
	pdflatex $(TARGET).tex
	bibtex $(TARGET)
	pdflatex $(TARGET).tex
	pdflatex $(TARGET).tex

edit:
	gedit Makefile *.bib *.tex &

clean:
	rm -f $(TARGET).pdf *.aux *.log *.blg *.bbl *.dvi *.ps *.toc *.lot *.lof *.idx *~

