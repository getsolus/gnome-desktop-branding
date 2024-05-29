gdm_schemas = [
    'org.gnome.settings-daemon.plugins.power.gschema.override'
]

custom_target('50_gnome_gdm.gschema.override',
    output: '50_gnome_gdm.gschema.override',
    capture: true,
    input: gdm_schemas,
    command: ['cat', '@INPUT@'],
    install: true,
    install_dir: path_gdmschemadir,
)
