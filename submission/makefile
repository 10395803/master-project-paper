PAPER=RBMNN_manuscript.tex
SNP=RBMNN_significance.tex
RH=RBMNN_highlights.tex
IMG_DIR=img
IMG=$(wildcard $(IMG_DIR)/*)

all: paper snp rh clear 

paper: $(PAPER) $(IMG)
	pdflatex $(PAPER)

snp: $(SNP)
	pdflatex $(SNP)

rh: $(RH)
	pdflatex $(RH)

PHONY: clear

clear:
	$(RM) *.log *.out *.spl

