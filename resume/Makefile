all: resume.html resume.pdf

%.html: %.md
	pandoc -c resume.css -B resumeB.html -A resumeA.html -o $@ $<

%.pdf: %.md
	pandoc -H resumeH.tex -o $@ $<

clean:
	rm -f *~ *.html *.log *.pdf
