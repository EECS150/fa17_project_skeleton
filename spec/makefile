srcdir  = .

main = spec
figs = $(wildcard images/*)

pdf : $(main).pdf
.PHONY: pdf

%.pdf: %.tex $(figs)
	texfot lualatex -shell-escape $(main).tex
	texfot lualatex -shell-escape $(main).tex

clean :
	rm -rf *.pdf *.aux *.out *.log _minted* *.pyg *.synctex.gz *.toc
