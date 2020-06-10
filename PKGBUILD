pkgbase=bootsplash-themes
pkgname=('bootsplash-theme-pine')
pkgver=1
pkgrel=1
url="https://lists.freedesktop.org/archives/dri-devel/2017-December/160242.html"
arch=('aarch64')
license=('GPL')

depends=()
builddepends=('imagemagick')
options=('!libtool' '!emptydirs')

source=('bootsplash-packer'
	'bootsplash-pine.sh'
	'bootsplash-pine.initcpio_install'
	'spinner.gif'
	'pine.png')

sha256sums=('9fee73278386fd713d0d7c67369e30fd02036df0addd62a83bf6c9f2ffb2eccc'
            '5f3285c20cf89d03cd7785abee254e5e6f725037b47d7abf6ab8a92feba6cd70'
            'f0347c1f1470b6a1fc3c10b2ab63596f6ca56be1a00d298153504a87698b83e8'
            '48a3b7ddc14be47609b77710d0bb0754718b6c9da5230183842a08fbd3b5a125'
            'da6cef4e5fb781ddef7d4dbed8bbb71d5313ada94748a5e3af2f51d3349c683a')

build() {
  cd "$srcdir"
  sh ./bootsplash-pine.sh
}

package_bootsplash-theme-pine() {
  pkgdesc="Bootsplash Theme with Pine logo"
  cd "$srcdir"

  install -Dm644 "$srcdir/bootsplash-pine" "$pkgdir/usr/lib/firmware/bootsplash-themes/pine/bootsplash"
  install -Dm644 "$srcdir/bootsplash-pine.initcpio_install" "$pkgdir/usr/lib/initcpio/install/bootsplash-pine"
} 
