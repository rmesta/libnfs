lib_LTLIBRARIES = libnfs.la

libnfs_la_CPPFLAGS = -I$(abs_top_srcdir)/include \
		     -I$(abs_top_srcdir)/include/nfsc \
		     -I../mount \
		     -I../nfs \
		     -I../nlm \
		     -I../portmap \
		     -I../rquota \
		     "-D_U_=__attribute__((unused))"

libnfs_la_SOURCES = \
	init.c \
	libnfs.c \
	libnfs-sync.c \
	libnfs-zdr.c \
	pdu.c \
	socket.c

libnfs_la_LDFLAGS = -version-info 1:7:0
libnfs_la_LIBADD = \
	../mount/libmount.la \
	../nfs/libnfs.la \
	../nlm/libnlm.la \
	../portmap/libportmap.la \
	../rquota/librquota.la 

