PAPER=RBMNN_manuscript_revised.tex
PUBLICATION=RBMNN_manuscript_publication.tex
REPLY=RBMNN_response_to_reviewers.tex
LIST=RBMNN_modifications.tex
IMG_DIR=img
IMG=$(wildcard $(IMG_DIR)/*)

all: paper publication reply list clear

paper: $(PAPER) $(IMG)
	pdflatex --shell-escape $(PAPER)

publication: $(PUBLICATION) $(IMG)
	pdflatex --shell-escape $(PUBLICATION)

reply: $(REPLY)
	pdflatex $(REPLY)

list: $(LIST)
	pdflatex $(LIST)

.PHONY: clean

clean:
	$(RM) *.log *.out *.spl

