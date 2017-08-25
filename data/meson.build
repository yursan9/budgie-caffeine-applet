gnome = import('gnome')

install_data(
    'CaffeineApplet.plugin',
    install_dir: APPLET_INSTALL_DIR
)

install_data(
    'caffeine-cup-empty.svg',
    install_dir: join_paths(ICON_INSTALL_DIR, 'scalable', 'status')
)
install_data(
    'caffeine-cup-full.svg',
    install_dir: join_paths(ICON_INSTALL_DIR, 'scalable', 'status')
)
install_data(
    'my-caffeine-on-symbolic.svg',
    install_dir: join_paths(ICON_INSTALL_DIR, 'symbolic', 'apps')
)

install_data(
    'com.github.yursan9.budgie-caffeine-applet.gschema.xml',
    install_dir: join_paths(datadir, 'glib-2.0', 'schemas'),
)

meson.add_install_script('meson_post_install')
