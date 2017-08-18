# asciidoctor
Unofficial [asciidoctor](https://github.com/asciidoctor/asciidoctor) docker image.

In addition to asciidoctor, the following has been installed.

- asciidoctor-diagram
- asciidoctor-mathematical
- asciidoctor-pdf
- asciidoctor-pdf-cjk

It is setup so that the diagram below can be used.

- erd
- ditaa
- graphviz
- latexmath
- plantuml

## How to use this image

### Convert asciidoc to html  

    docker run -it --rm -v $(pwd):$(pwd) -w $(pwd) cosmicvelocity/asciidoctor:1.5.6.1 asciidoctor -b html5 -r asciidoctor-diagram sample.adoc

### Convert asciidoc to pdf

    docker run -it --rm -v $(pwd):$(pwd) -w $(pwd) cosmicvelocity/asciidoctor:1.5.6.1 asciidoctor-pdf -r asciidoctor-diagram -a toc -n sample.adoc

### Convert asciidoc to pdf (contains mathematical).

    docker run -it --rm -v $(pwd):$(pwd) -w $(pwd) cosmicvelocity/asciidoctor:1.5.6.1 asciidoctor-pdf -r asciidoctor-mathematical sample.adoc

## License
View license information for the software contained in this image.

- [asciidoctor](https://github.com/asciidoctor/asciidoctor/blob/master/LICENSE.adoc)
- [asciidoctor-diagram](https://github.com/asciidoctor/asciidoctor-diagram/blob/master/LICENSE.txt)
- [asciidoctor-mathematical](https://github.com/asciidoctor/asciidoctor-mathematical/blob/master/LICENSE)
- [asciidoctor-pdf](https://github.com/asciidoctor/asciidoctor-pdf/blob/master/LICENSE.adoc)
- [asciidoctor-pdf-cjk](https://github.com/chloerei/asciidoctor-pdf-cjk/blob/master/LICENSE.txt)
- [erd](https://github.com/BurntSushi/erd/blob/master/UNLICENSE)
- [graphviz](http://www.graphviz.org/License.php)
- [openjdk](http://openjdk.java.net/legal/gplv2+ce.html)
- [IPAexフォント](http://ipafont.ipa.go.jp/ipa_font_license_v1-html)
- [noto-cjk](https://github.com/googlei18n/noto-cjk/blob/master/LICENSE)
