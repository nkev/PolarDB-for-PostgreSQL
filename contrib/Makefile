# contrib/Makefile

subdir = contrib
top_builddir = ..
include $(top_builddir)/src/Makefile.global

SUBDIRS = \
		adminpack	\
		amcheck		\
		auth_delay	\
		auto_explain	\
		bloom		\
		btree_gin	\
		btree_gist	\
		citext		\
		cube		\
		dblink		\
		dict_int	\
		dict_xsyn	\
		earthdistance	\
		file_fdw	\
		fuzzystrmatch	\
		hstore		\
		intagg		\
		intarray	\
		isn		\
		lo		\
		ltree		\
		oid2name	\
		passwordcheck	\
		pg_buffercache	\
		pgxc_ctl	\
		pg_freespacemap \
		pg_prewarm	\
		pg_standby	\
		pg_stat_statements \
		pg_trgm		\
		pgcrypto	\
		pgrowlocks	\
		pg_visibility	\
		postgres_fdw	\
		seg		\
		spi		\
		tablefunc	\
		tcn		\
		tsm_system_rows \
		tsm_system_time \
		unaccent	\
		polar_monitor \
		vacuumlo

ifeq ($(with_openssl),yes)
SUBDIRS += sslinfo
else
ALWAYS_SUBDIRS += sslinfo
endif

ifneq ($(with_uuid),no)
SUBDIRS += uuid-ossp
else
ALWAYS_SUBDIRS += uuid-ossp
endif

ifeq ($(with_libxml),yes)
SUBDIRS += xml2
else
ALWAYS_SUBDIRS += xml2
endif

ifeq ($(with_selinux),yes)
SUBDIRS += sepgsql
else
ALWAYS_SUBDIRS += sepgsql
endif

ifeq ($(with_perl),yes)
SUBDIRS += hstore_plperl jsonb_plperl
else
ALWAYS_SUBDIRS += hstore_plperl jsonb_plperl
endif

ifeq ($(with_python),yes)
SUBDIRS += hstore_plpython jsonb_plpython ltree_plpython
else
ALWAYS_SUBDIRS += hstore_plpython jsonb_plpython ltree_plpython
endif

# Missing:
#		start-scripts	\ (does not have a makefile)


$(recurse)
$(recurse_always)
