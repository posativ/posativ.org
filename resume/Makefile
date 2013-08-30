all: resume.html resume.pdf

%.html: %.md resume.css resumeB.html resumeA.html
	pandoc -c resume.css -B resumeB.html -A resumeA.html -o $@ $<

%.pdf: %.md resumeH.tex
	pandoc -H resumeH.tex -o $@ $<

clean:
	rm -f *~ *.html *.log *.pdf
