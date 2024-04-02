CSSDIR=css
IMAGESDIR=images
.SUFFIXES:
.SUFFIXES: adoc html

%.html: %.adoc
	asciidoctor -b html5 -a linkcss -a imagesdir=$(IMAGESDIR) -a stylesdir=$(CSSDIR)  -r asciidoctor-html5s \
	-a stylesheet=asciidoctor.css -a topics=../topics $< -o $(@F)


VPATH=../sources/docs:../sources/topics

include depfile
#index.html: ../sources/docs/index.adoc

