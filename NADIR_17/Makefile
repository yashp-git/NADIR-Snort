release:
	make clean
	make NADIR.pdf

zip:
	/bin/rm -f *.aux *.bbl *.blg *.log *~
	(cd ..;zip latex-templates.zip latex-templates/*)

NADIR.pdf: NADIR.tex NADIR.bib
		pdflatex NADIR
		bibtex NADIR
		pdflatex NADIR
		pdflatex NADIR
clean:
	rm -f NADIR.{bbl,blg,log,pdf}
