PDFS=components.pdf

all: $(PDFS)

components.pdf: components.tikz

%.pdf: %.md ../article.template
	pandoc $< -o $@ \
	--template=../article.template \
	--chapters \
	--latex-engine=lualatex
