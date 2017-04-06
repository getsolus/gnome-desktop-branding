SUBDIRS = \
	extensions

LIVECD_SCHEMAS = \
	com.solus-project.software-center.gschema.override \
	org.gnome.desktop.screensaver.gschema.override \
	org.gnome.shell.gschema.override

%.gschema.override:
	rm -f $@ ;
	for i in ${LIVECD_SCHEMAS} ; do \
	    cat $${i} >> $@; \
	    echo  >> $@; \
	done ;

EXTRA_DIST = \
	$(LIVECD_SCHEMAS)

overridesdir = \
	$(datadir)/glib-2.0/schemas

overrides_DATA = \
	20_gnome_livecd.gschema.override

distclean-local:
	rm -fv ${top_builddir}/schemas/livecd/20_gnome_livecd.gschema.override
