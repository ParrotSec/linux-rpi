include $(top_rulesdir)/Makefile.inc

ifneq ($(filter i386 amd64 x32 arm64,$(DEB_HOST_ARCH)),)

all:
	$(MAKE_UPSTREAM)

install:
	$(MAKE_UPSTREAM) install
	rm -f $(DESTDIR)/usr/libexec/hypervkvpd/hv_set_ifconfig \
		$(DESTDIR)/usr/sbin/lsvmbus

endif
