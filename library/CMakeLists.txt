cmake_minimum_required(VERSION 3.12)

set(SOURCES  common.c ioconf.c rd_stats.c count.c)
set(HEADERS common.h ioconf.h rd_stats.h count.h)

add_library(lib ${SOURCES} ${HEADERS})
