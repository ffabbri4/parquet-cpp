lib_LTLIBRARIES = libparquet.la

include_HEADERS = parquet/parquet.h

libparquet_la_CPPFLAGS = -I$(top_srcdir)/generated $(THRIFT_CFLAGS)
libparquet_la_LIBADD = ../generated/libgenerated.la

nobase_include_HEADERS = 	compression/codec.h \
	encodings/bool-encoding.h \
	encodings/delta-bit-pack-encoding.h \
	encodings/delta-byte-array-encoding.h \
	encodings/delta-length-byte-array-encoding.h \
	encodings/dictionary-encoding.h \
	encodings/encodings.h \
	encodings/plain-encoding.h \
	impala/bit-stream-utils.h \
	impala/bit-stream-utils.inline.h \
	impala/bit-util.h \
	impala/compiler-util.h \
	impala/logging.h \
	impala/rle-encoding.h \
	parquet/parquet.h \
	util/stopwatch.h

libparquet_la_SOURCES = \
	compression/lz4-codec.cc \
	compression/snappy-codec.cc \
	parquet.cc




 
