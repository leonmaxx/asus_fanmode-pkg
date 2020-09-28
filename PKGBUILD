# Maintainer: Leonid Maksymchuk <leonmaxx@gmail.com>
pkgname=asus_fanmode
pkgver=0.3.1
pkgrel=1
pkgdesc="Daemon that controls Fan Boost Mode on ASUS TUF laptops"
arch=('x86_64')
url="https://github.com/leonmaxx/asus_fanmode"
license=('BSD')
source=(https://github.com/leonmaxx/asus_fanmode/archive/v${pkgver}.tar.gz)
md5sums=('59c37676f23c29cabea2d893cefaed10')
makedepends=(make gcc)

build() {
  cd "${pkgname}-${pkgver}"
  make CXXFLAGS="$CXXFLAGS"
}

package() {
  cd "${pkgname}-${pkgver}"
  make install DESTDIR="$pkgdir"
}
