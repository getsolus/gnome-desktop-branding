GNOME_SCHEMAS = \
	com.worldwidemann.plotinus.gschema.override \
	org.gnome.desktop.background.gschema.override \
	org.gnome.desktop.interface.gschema.override \
	org.gnome.desktop.screensaver.gschema.override \
	org.gnome.desktop.wm.preferences.gschema.override \
	org.gnome.nautilus.icon-view.gschema.override \
	org.gnome.settings-daemon.plugins.xsettings.gschema.override \
	org.gnome.shell.extensions.dash-to-dock.gschema.override \
	org.gnome.shell.extensions.topicons.gschema.override \
	org.gnome.shell.extensions.user-theme.gschema.override \
	org.gnome.shell.gschema.override \
	org.gtk.settings.file-chooser.gschema.override

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
	10_gnome_settings.gschema.override

distclean-local:
	rm -fv ${top_builddir}/schemas/gnome/10_gnome_settings.gschema.override
