TEX = pdflatex -interaction nonstopmode

PAPER = trustzone

all:	$(PAPER).pdf

view:	$(PAPER).pdf
	gnome-open $(PAPER).pdf

spell::
	ispell *.tex

clean::
	rm -fv *.aux *.log *.bbl *.blg *.toc *.out *.lot *.lof *.pdf *.gz

$(PAPER).pdf: $(PAPER).tex
	-$(TEX) $(PAPER)
	$(TEX) $(PAPER)
