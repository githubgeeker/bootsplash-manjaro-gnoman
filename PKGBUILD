pkgbase=bootsplash-themes
pkgname=('bootsplash-manjaro-gnoman')
pkgver=1
pkgrel=1
url="https://lists.freedesktop.org/archives/dri-devel/2017-December/160242.html"
arch=('x86_64')
license=('GPL')

depends=()
builddepends=('imagemagick')
options=('!libtool' '!emptydirs')

source=('bootsplash-packer'
    'bootsplash-packer.rst'
	'bootsplash-manjaro-gnoman.sh'
	'bootsplash-manjaro-gnoman.initcpio_install'
	'README.md'
	'logo.png'
	'spinner.gif')

sha256sums=('51559d3ccfb448b03fa6439faf5869dbd0c2fbda1b5d5bf5d4ba70e60937472a'
            '35596e3f9c62d5f50730992befb940bfa75a24a2da15b558364300b52b64aa87'
            '05bd04f0e4fd56f06cc1df09cf9b325c1e2f6f91213097fbbf9c2cb08308a1b2'
            'ab094dbf6779cbee02efadc872fe9ab61c29a8235f806e9a542fe2324da3c433'
            '0cc9f1329098154bb11f20b4aa1d7f99eed1727b9e203fc6c698d64c6f123308'
            '64fcb25871f7afc84d814cca2fade3b11cff47278198a5f2e92ae44010354b55'
            'd070284d3a780216068f7833b34a38d9ef8d42e95bdf77f0e88a36fcc5732b26')

build() {
  cd "$srcdir"
  sh ./bootsplash-manjaro-gnoman.sh
}

package_bootsplash-manjaro-gnoman() {
  pkgdesc="Bootsplash Theme with Gnoman"
  cd "$srcdir"

  install -Dm644 "$srcdir/bootsplash-manjaro-gnoman" "$pkgdir/usr/lib/firmware/bootsplash-themes/manjaro-gnoman/bootsplash"
  install -Dm644 "$srcdir/bootsplash-manjaro-gnoman.initcpio_install" "$pkgdir/usr/lib/initcpio/install/bootsplash-manjaro-gnoman"
} 
