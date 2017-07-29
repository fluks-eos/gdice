include $(top_srcdir)/common.mk

generated_parser_files = lex.yy.c de.tab.c de.tab.h

bin_PROGRAMS = com.github.fluks-eos.gdice
com_github_fluks_eos_gdice_SOURCES = \
	main.c 		\
	diceexpr.h 	\
	numflow.h 	\
	sound.c 	\
	sound.h 	\
	str.c 		\
	str.h

nodist_com_github_fluks_eos_gdice_SOURCES = $(generated_parser_files)

lex.yy.c: de.l
	$(LEX) $<

de.tab.c: de.y str.o
	bison --defines=de.tab.h $<

BUILT_SOURCES = $(generated_parser_files)
EXTRA_DIST = de.l de.y
CLEANFILES = $(generated_parser_files)
