desktopdir 	 = $(datadir)/applications
desktop_in_files = xed.desktop.in
desktop_DATA 	 = $(desktop_in_files:.desktop.in=.desktop)
@INTLTOOL_DESKTOP_RULE@

@INTLTOOL_XML_RULE@
appdatadir = $(datadir)/appdata
appdata_in_files = xed.appdata.xml.in
appdata_DATA = $(appdata_in_files:.xml.in=.xml)

gsettings_SCHEMAS = org.x.editor.gschema.xml
@GSETTINGS_RULES@

man_MANS = xed.1

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = xed.pc

bugreportdir = $(libexecdir)/xed
bugreport_SCRIPTS = xed-bugreport.sh

EXTRA_DIST = 			\
	$(appdata_in_files)	\
	$(desktop_in_files)	\
	$(man_MANS)			\
	xed.pc.in			\
	xed-bugreport.sh.in

CLEANFILES =	 			\
	$(desktop_DATA)			\
	$(gsettings_SCHEMAS)	\
	$(pkgconfig_DATA)		\
	$(appdata_DATA)




-include $(top_srcdir)/git.mk
