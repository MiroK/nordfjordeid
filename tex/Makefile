.PHONY: all clean

all: precond.pdf coupled.pdf

precond.pdf: precond.tex
	latexmk -pdfps -pdflatex="pdflatex --shell-escape %O %S" $<

coupled.pdf: coupled.tex
	latexmk -pdfps -pdflatex="pdflatex --shell-escape %O %S" $<

view: 
	evince precond.pdf &
	evince coupled.pdf &

clean:
	latexmk -C
