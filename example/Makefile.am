bin_PROGRAMS = compute_stats decode_benchmark 

compute_stats_SOURCES = compute_stats.cc example_util.cc example_util.h
compute_stats_CPPFLAGS = -I$(top_srcdir)/generated -I$(top_srcdir)/src $(THRIFT_CFLAGS)
compute_stats_LDADD = ../src/libparquet.la
compute_stats_LDFLAGS = $(THRIFT_LIBS)

decode_benchmark_SOURCES = decode_benchmark.cc example_util.cc example_util.h
decode_benchmark_CPPFLAGS = -I$(top_srcdir)/generated -I$(top_srcdir)/src $(THRIFT_CFLAGS)
decode_benchmark_LDADD = ../src/libparquet.la
decode_benchmark_LDFLAGS = $(THRIFT_LIBS)
