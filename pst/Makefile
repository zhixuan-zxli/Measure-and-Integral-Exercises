
.PHONY : allEps clean realclean

allEps : convGraph_1.pdf convGraph_2.pdf convGraph_3.pdf

clean :
	rm -f *.dvi *.aux *.log *~

realclean :
	rm -f *.dvi *.aux *.log *~ *.ps *.pdf

%.pdf : %.ps
	ps2pdf $<

%.ps : %.dvi
	dvips $<

%.dvi : %.tex
	latex $<
