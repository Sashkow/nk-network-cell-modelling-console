SUBDIRS = cell_modelling

bin_SCRIPTS = nk-network-cell-modelling
CLEANFILES = $(bin_SCRIPTS)
EXTRA_DIST = nk-network-cell-modelling.in

do_substitution = sed -e 's,[@]pythondir[@],$(pythondir),g' \
	-e 's,[@]PACKAGE[@],$(PACKAGE),g' \
	-e 's,[@]VERSION[@],$(VERSION),g' 

nk-network-cell-modelling: nk-network-cell-modelling.in Makefile
	$(do_substitution) < $(srcdir)/nk-network-cell-modelling.in > nk-network-cell-modelling
	chmod +x nk-network-cell-modelling