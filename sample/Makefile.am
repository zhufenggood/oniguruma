#noinst_PROGRAMS = encode listcap names posix simple sql syntax crnl

lib_onig = ../src/libonig.la
LDADD  = $(lib_onig)

AM_LDFLAGS  = -L$(prefix)/lib
AM_CPPFLAGS = -I../src -I$(includedir)

TESTS = encode listcap names posix simple sql syntax user_property

check_PROGRAMS = encode listcap names posix simple sql syntax user_property

encode_SOURCES  = encode.c
listcap_SOURCES = listcap.c
names_SOURCES   = names.c
posix_SOURCES   = posix.c
simple_SOURCES  = simple.c
sql_SOURCES     = sql.c
syntax_SOURCES  = syntax.c
user_property_SOURCES = user_property.c

sampledir = .

test: encode listcap names posix simple sql syntax user_property
	$(sampledir)/encode
	$(sampledir)/listcap
	$(sampledir)/names
	$(sampledir)/posix
	$(sampledir)/simple
	$(sampledir)/sql
	$(sampledir)/syntax
	$(sampledir)/user_property
