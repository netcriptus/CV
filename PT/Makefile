FILE=Fernando_Cezar_PT
TEX=${FILE}.tex
DVI=${FILE}.dvi
PS=${FILE}.ps
OUTPUT=Fernando_Cezar.pdf

ALL: ${PS}
	ps2pdf ${PS}
	mv ${FILE}.pdf ${OUTPUT}


${PS}: ${DVI}
	dvips ${DVI}

${DVI}: ${TEX}
	latex ${TEX}

${TEX}:
	echo ${FILE}
	latex ${TEX}


clean:
	rm -rf *.aux *.log *.out *.ps *.dvi *~