RM            = rm -rf
SPHINXOPTS    = -d .doctrees
SPHINXBUILD   = sphinx-build
AUTOBUILD     = sphinx-autobuild
SOURCEDIR     = .
BUILDDIR      = ../gh-pages

.PHONY = docs server clean invclean

docs:
	$(SPHINXBUILD) -b html "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS)
	touch $(BUILDDIR)/.nojekyll


server:
	@$(AUTOBUILD) "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) --watch ../aiopluggy --watch ./


clean:
	@$(RM) $(BUILDDIR) .doctrees


invclean:
	@$(RM) *.inv *.inv.txt
