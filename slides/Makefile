NOTEBOOKS:=$(wildcard *.ipynb)
SLIDES:=$(subst ipynb,slides.html,$(NOTEBOOKS))
HTML:=$(subst ipynb,html,$(NOTEBOOKS))
PDFS:=$(subst ipynb,pdf,$(NOTEBOOKS))

$(SLIDES): %.slides.html: %.ipynb
	jupyter nbconvert $< --to slides --reveal-prefix "http://cdnjs.cloudflare.com/ajax/libs/reveal.js/3.3.0"

slides:
	make $(SLIDES)

#pdfs:
#	make $(PDFS)

clean:
	rm *.html *.pdf

all:
	make slides
