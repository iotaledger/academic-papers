MAIN=main
LONG=Coordicide_WP

.PHONY: FORCE_MAKE
run: $(LONG).pdf

$(LONG).pdf: $(MAIN).tex FORCE_MAKE
	latexmk -pdf -dvi- -ps- -bibtex $<
	mv $(MAIN).pdf $(LONG).pdf

clean:
	rm -rf *.aux *.lof *.log *.lot *.toc *.bbl *.blg *pdf
