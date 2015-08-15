# Maintainer: SpepS <dreamspepser at yahoo dot it>
# Contributor: Alexander Fehr <pizzapunk gmail com>

pkgname=galculator
pkgver=1.3.4
pkgrel=2
pkgdesc="GTK+ based scientific calculator"
arch=('i686' 'x86_64')
url="http://galculator.sourceforge.net/"
license=('GPL')
depends=('libglade')
makedepends=('intltool')
install="$pkgname.install"
source=("http://downloads.sourceforge.net/galculator/galculator-$pkgver.tar.bz2")
md5sums=('d30e6fbf5947bb1c873bc9d5a21046f1')

build() {
  cd "$srcdir/$pkgname-$pkgver"

  ./configure --prefix=/usr
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"

  make DESTDIR="$pkgdir" install
}
