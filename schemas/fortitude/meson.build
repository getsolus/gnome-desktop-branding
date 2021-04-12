fortitude_schemas = [
    'org.gnome.desktop.background.gschema.override',
    'org.gnome.desktop.interface.gschema.override',
    'org.gnome.desktop.screensaver.gschema.override',
    'org.gnome.desktop.wm.preferences.gschema.override',
    'org.gnome.gedit.preferences.editor.override',
    'org.gnome.nautilus.icon-view.gschema.override',
    'org.gnome.nautilus.list-view.gschema.override',
    'org.gnome.nautilus.preferences.gschema.override',
    'org.gnome.settings-daemon.plugins.xsettings.gschema.override',
    'org.gnome.shell.extensions.trayIconsReloaded.gschema.override',
    'org.gnome.shell.extensions.user-theme.gschema.override',
    'org.gnome.shell.gschema.override',
    'org.gtk.settings.file-chooser.gschema.override',
]

custom_target('30_gnome_fortitude_settings.gschema.override',
    output: '30_gnome_fortitude_settings.gschema.override',
    capture: true,
    input: fortitude_schemas,
    command: ['cat', '@INPUT@'],
    install: true,
    install_dir: path_schemadir,
)
