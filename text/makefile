TEXT = ecograms
REFS = refs

all: $(TEXT).pdf

%.pdf: %.Rmd $(REFS).bib
	Rscript -e "rmarkdown::render('$<')"
	cp $@ ~/Dropbox/temp/

continuous:
	while true; do make --silent; sleep 3; done
