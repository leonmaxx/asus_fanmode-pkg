# Maintainer: Leonid Maksymchuk <leonmaxx@gmail.com>
pkgname=asus_fanmode
pkgver=0.1.0
pkgrel=1
pkgdesc="Daemon that controls Fan Boost Mode on ASUS TUF laptops"
arch=('x86_64')
url="https://github.com/leonmaxx/asus_fanmode"
license=('BSD')
source=(https://github.com/leonmaxx/asus_fanmode/archive/v${pkgver}.tar.gz)
md5sums=('b275ef69fa17a9ca73ec98cdf216ea2a')

build() {
  cd "${pkgname}-${pkgver}"
  make CXXFLAGS="$CXXFLAGS"
}

package() {
  cd "${pkgname}-${pkgver}"
  make install DESTDIR="$pkgdir"
}
