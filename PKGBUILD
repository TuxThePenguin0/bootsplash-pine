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

sha256sums=('SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP')

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
