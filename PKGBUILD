# Maintainer: Leonid Maksymchuk <leonmaxx@gmail.com>
pkgname=asus_fanmode
pkgver=0.3.0
pkgrel=2
pkgdesc="Daemon that controls Fan Boost Mode on ASUS TUF laptops"
arch=('x86_64')
url="https://github.com/leonmaxx/asus_fanmode"
license=('BSD')
source=(https://github.com/leonmaxx/asus_fanmode/archive/v${pkgver}.tar.gz)
md5sums=('421c90efdfb6f9b3335665ea23354cbe')

build() {
  cd "${pkgname}-${pkgver}"
  make CXXFLAGS="$CXXFLAGS"
}

package() {
  cd "${pkgname}-${pkgver}"
  make install DESTDIR="$pkgdir"
}
