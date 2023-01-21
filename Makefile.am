SUBDIRS = src test

man_MANS = man/stress.1

EXTRA_DIST= autogen.sh CONTRIBUTING.md man/stress.1 doc/stress.png README.md

distclean-local:
	rm -rf autom4te.cache
	rm -f  aclocal.m4 compile config.* configure depcomp INSTALL install-sh \
               Makefile.in missing src/Makefile.in test-driver test/Makefile.in
