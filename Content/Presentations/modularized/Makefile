LATEXMK = latexmk -lualatex
LATEXMK-C = latexmk -c

default: all

workaround-on:
	sed -i.bak 's|%\\input|\\input|g' KokkosTutorial_PreTitle.tex
	rm KokkosTutorial_PreTitle.tex.bak

workaround-off:
	sed -i.bak 's|\\input|%\\input|g' KokkosTutorial_PreTitle.tex
	sed -i.bak 's|%%\\input|%\\input|g' KokkosTutorial_PreTitle.tex
	rm KokkosTutorial_PreTitle.tex.bak

overview:
	$(LATEXMK) Kokkos_ShortOverview
short:
	$(LATEXMK) KokkosTutorial_Short
medium:
	$(LATEXMK) KokkosTutorial_Medium
module1:
	$(LATEXMK) KokkosTutorial_01_Introduction
module2:
	$(LATEXMK) KokkosTutorial_02_ViewsAndSpaces
module3:
	$(LATEXMK) KokkosTutorial_03_MDRangeMoreViews
module4:
	$(LATEXMK) KokkosTutorial_04_HierarchicalParallelism
module5:
	$(LATEXMK) KokkosTutorial_05_SIMDStreamsTasking
module6:
	$(LATEXMK) KokkosTutorial_06_InternodeMPIAndPGAS
module7:
	$(LATEXMK) KokkosTutorial_07_Tools
module8:
	$(LATEXMK) KokkosTutorial_08_KokkosKernels
module9:
	$(LATEXMK) KokkosTutorial_09_Fortran

all: module1 module2 module3 module4 module5 module6 module7 module8 module9

clean:
	$(LATEXMK-C)
