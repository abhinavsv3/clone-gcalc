SUBDIRS = po src data help

# Temporary fix for JHBuild, see https://bugzilla.gnome.org/show_bug.cgi?id=641652
ACLOCAL_AMFLAGS = ${ACLOCAL_FLAGS} -I m4

DISTCLEANFILES = test-driver

MAINTAINERCLEANFILES = \
	$(GITIGNORE_MAINTAINERCLEANFILES_TOPLEVEL) \
	$(GITIGNORE_MAINTAINERCLEANFILES_MAKEFILE_IN)

EXTRA_DIST = \
	autogen.sh \
	gnome-calculator.doap

@BEHAVE_INSTALLED_TESTS_RULE@
INSTALLED_TESTS=basic_mode advanced_mode financial_mode programming_mode
INSTALLED_TESTS_TYPE=session-exclusive

-include $(top_srcdir)/git.mk
