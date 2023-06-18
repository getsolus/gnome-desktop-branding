gnome_schemas = [
    'org.gnome.desktop.background.gschema.override',
    'org.gnome.desktop.interface.gschema.override',
    'org.gnome.desktop.screensaver.gschema.override',
    'org.gnome.desktop.wm.preferences.gschema.override',
    'org.gnome.gedit.preferences.editor.override',
    'org.gnome.nautilus.icon-view.gschema.override',
    'org.gnome.nautilus.list-view.gschema.override',
    'org.gnome.nautilus.preferences.gschema.override',
    'org.gnome.shell.extensions.trayIconsReloaded.gschema.override',
    'org.gnome.shell.gschema.override',
    'org.gtk.settings.file-chooser.gschema.override',
]

custom_target('30_gnome_settings.gschema.override',
    output: '30_gnome_settings.gschema.override',
    capture: true,
    input: gnome_schemas,
    command: ['cat', '@INPUT@'],
    install: true,
    install_dir: path_schemadir,
)

subdir('livecd')
