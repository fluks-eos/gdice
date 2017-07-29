SUBDIRS = \
	32 \
	48 \
	64 \
	128

resdir = $(datadir)/@PACKAGE_NAME@
dist_res_DATA = \
	gdice.svg \
	add_12x12.svg \
	dices.ogg \
	gdice.glade \
	remove_12x12.svg \
	gdice.css

desktopdir = $(datadir)/applications
desktop_in_files = com.github.fluks-eos.gdice.desktop.in
dist_desktop_DATA = $(desktop_in_files:.desktop.in=.desktop)
@INTLTOOL_DESKTOP_RULE@

metainfodir = $(datadir)/metainfo
dist_metainfo_DATA = com.github.fluks-eos.gdice.appdata.xml

gsettings_SCHEMAS = com.github.fluks-eos.gdice.gschema.xml
EXTRA_DIST = $(gsettings_SCHEMAS)
@GSETTINGS_RULES@

DISTCLEANFILES = \
	$(desktop_DATA)
