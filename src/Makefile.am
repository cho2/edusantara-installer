NULL = 

AM_CPPFLAGS = \
    -DLIBSOUP_USE_UNSTABLE_REQUEST_API \
	$(INSTALLER_CFLAGS) \
	-include config.h \
	-DLOCALEDIR=\""$(localedir)"\" \
	-DPKGDATADIR=\""$(pkgdatadir)"\" \
	$(NULL)

bin_PROGRAMS = edusantara-installer

edusantara_installer_SOURCES = \
    main.vala \
	installer.vala \
	parted.vala \
    utils.vala \
	$(NULL)

edusantara_installer_VALAFLAGS = \
    --vapidir ../vapi \
	--pkg config \
    $(VALA_PACKAGES) \
    $(NULL)

edusantara_installer_LDADD = \
	$(INSTALLER_LIBS) \
	$(NULL)

desktopdir = $(prefix)/share/applications
dist_desktop_DATA = edusantara-installer.desktop

EXTRA_DIST = \
	$(NULL)

DISTCLEANFILES = \
	$(NULL)


