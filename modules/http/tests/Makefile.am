if ENABLE_HTTP

modules_http_tests_TESTS			= \
	modules/http/tests/test_http			\
	modules/http/tests/test_http-loadbalancer	\
	modules/http/tests/test_http-response_handlers	\
	modules/http/tests/test_http-signal_slot	\
	modules/http/tests/test_compression

check_PROGRAMS					+= ${modules_http_tests_TESTS}

EXTRA_modules_http_tests_test_http_DEPENDENCIES =      \
        $(top_builddir)/modules/http/libhttp.la
modules_http_tests_test_http_CFLAGS	= $(TEST_CFLAGS) -I$(top_srcdir)/modules/http
modules_http_tests_test_http_LDADD	= $(TEST_LDADD) $(PREOPEN_BASICFUNCS)
modules_http_tests_test_http_LDFLAGS	= \
	-dlpreopen $(top_builddir)/modules/http/libhttp.la


EXTRA_modules_http_tests_test_http_loadbalancer_DEPENDENCIES = \
	$(top_builddir)/modules/http/libhttp.la
modules_http_tests_test_http_loadbalancer_CFLAGS	= $(TEST_CFLAGS) -I$(top_srcdir)/modules/http
modules_http_tests_test_http_loadbalancer_LDADD		= $(TEST_LDADD)
modules_http_tests_test_http_loadbalancer_LDFLAGS	= \
	-dlpreopen $(top_builddir)/modules/http/libhttp.la


EXTRA_modules_http_tests_test_http_response_handlers_DEPENDENCIES = \
	$(top_builddir)/modules/http/libhttp.la
modules_http_tests_test_http_response_handlers_CFLAGS	= $(TEST_CFLAGS) -I$(top_srcdir)/modules/http
modules_http_tests_test_http_response_handlers_LDADD = $(TEST_LDADD)
modules_http_tests_test_http_response_handlers_LDFLAGS	= \
	-dlpreopen $(top_builddir)/modules/http/libhttp.la

EXTRA_modules_http_tests_test_http_signal_slot_DEPENDENCIES = \
	$(top_builddir)/modules/http/libhttp.la
modules_http_tests_test_http_signal_slot_CFLAGS	= $(TEST_CFLAGS) -I$(top_srcdir)/modules/http
modules_http_tests_test_http_signal_slot_LDADD = $(TEST_LDADD)
modules_http_tests_test_http_signal_slot_LDFLAGS	= \
	-dlpreopen $(top_builddir)/modules/http/libhttp.la

EXTRA_modules_http_tests_test_compression_DEPENDENCIES = \
	$(top_builddir)/modules/http/libhttp.la
modules_http_tests_test_compression_CFLAGS	= $(TEST_CFLAGS) -I$(top_srcdir)/modules/http
modules_http_tests_test_compression_LDADD = $(TEST_LDADD)
modules_http_tests_test_compression_LDFLAGS	= \
	-dlpreopen $(top_builddir)/modules/http/libhttp.la
endif

EXTRA_DIST += modules/http/tests/CMakeLists.txt
