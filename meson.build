project('budgie-caffeine-applet',
	version: '0.1.0',
	meson_version: '>= 0.40.0'
)

i18n = import('i18n')
python = import('python3')

message('Looking for dependencies')
python_bin = python.find_python()
if not python_bin.found()
	error('No python3 binary found')
else
	message('Found python3 binary')
endif
dependency('glib-2.0')
dependency('budgie-1.0', version: '>=2')
dependency('gobject-introspection-1.0', version: '>=1.51.1')
dependency('gtk+-3.0', version :'>=3.22')

# Global path variabel
prefix = get_option('prefix')
libdir = join_paths(prefix, get_option('libdir'))
datadir = join_paths(prefix, get_option('datadir'))
ICON_INSTALL_DIR = join_paths(datadir, 'icons', 'hicolor')
APPLET_INSTALL_DIR = join_paths(libdir, 'budgie-desktop',
	'plugins', meson.project_name())

conf = configuration_data()
conf.set('PROJECT_NAME', meson.project_name())

message('Installing applet...')
subdir('data')
configure_file(
	input: meson.project_name() + '.py.in',
	output: meson.project_name() + '.py',
	configuration: conf,
	install_dir: APPLET_INSTALL_DIR
)
