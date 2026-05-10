LATEXMK = latexmk -lualatex
LATEXMK-C = latexmk -c

default: release-51

workaround-on:
	sed -i.bak 's|%\\input|\\input|g' KokkosTutorial_PreTitle.tex
	rm KokkosTutorial_PreTitle.tex.bak

workaround-off:
	sed -i.bak 's|\\input|%\\input|g' KokkosTutorial_PreTitle.tex
	sed -i.bak 's|%%\\input|%\\input|g' KokkosTutorial_PreTitle.tex
	rm KokkosTutorial_PreTitle.tex.bak

release-36:
	$(LATEXMK) release-36

release-37:
	$(LATEXMK) release-37

release-40:
	$(LATEXMK) release-40

release-41:
	$(LATEXMK) release-41

release-42:
	$(LATEXMK) release-42

release-43:
	$(LATEXMK) release-43

release-44:
	$(LATEXMK) release-44

release-45:
	$(LATEXMK) release-45

release-46:
	$(LATEXMK) release-46

release-47:
	$(LATEXMK) release-47

release-50:
	$(LATEXMK) release-50

release-51:
	$(LATEXMK) release-51

all: release-36 release-37 release-40 release-41 release-42 release-43 release-44 release-45 release-46 release-47 release-50 release-51

clean:
	$(LATEXMK-C)
