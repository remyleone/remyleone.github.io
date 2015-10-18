all:
	latexmk -jobname=en
	mv en.pdf ../cv_en_leone_remy.pdf
	latexmk -jobname=fr
	mv fr.pdf ../cv_fr_leone_remy.pdf

clean:
	latexmk -C
