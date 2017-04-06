GNOME_SCHEMAS = \
	org.gnome.shell.extensions.dash-to-dock.gschema.override \
	org.gnome.shell.extensions.dynamic-panel-transparency.gschema.override \
	org.gnome.shell.extensions.topicons.gschema.override \
	org.gnome.shell.extensions.user-theme.gschema.override

%.gschema.override:
	rm -f $@ ;
	for i in ${GNOME_SCHEMAS} ; do \
	    cat $${i} >> $@; \
	    echo  >> $@; \
	done ;

EXTRA_DIST = \
	$(GNOME_SCHEMAS)

overridesdir = \
	$(datadir)/glib-2.0/schemas

overrides_DATA = \
	10_gnome_extensions.gschema.override

distclean-local:
	rm -fv ${top_builddir}/schemas/gnome/10_gnome_extensions.gschema.override