BENCHCFLAGS = $(AM_CFLAGS)  -I.. @CFLAGS@ -DNDEBUG
BENCHLIBADD = -lmpfr -lgmp -lm
BENCHLDFLAGS = -Wl,-rpath,../.libs/ ../.libs/libdgs.la

bin_PROGRAMS = bench_gauss bench_rround

.PHONY: clean dist-clean

bench_gauss_SOURCES=bench_gauss.c bench.c bench.h
bench_gauss_CFLAGS=${BENCHCFLAGS}
bench_gauss_LDFLAGS=${BENCHLDFLAGS} ${BENCHLIBADD}

bench_rround_SOURCES=bench_rround.c bench.c bench.h
bench_rround_CFLAGS=${BENCHCFLAGS}
bench_rround_LDFLAGS=${BENCHLDFLAGS} ${BENCHLIBADD}

