pkgname=tree
pkgver=2.2.1
pkgrel=2
pkgdesc="A directory listing program displaying a depth indented list of files"
arch=('x86_64')
url="http://oldmanprogrammer.net/source.php?dir=projects/tree"
license=('GPL')
depends=('glibc')
source=("https://github.com/Old-Man-Programmer/${pkgname}/archive/refs/tags/${pkgver}.tar.gz")
sha256sums=('5caddcbca805131ff590b126d3218019882e4ca10bc9eb490bba51c05b9b3b75')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make PREFIX="${pkgdir}/usr" MANDIR="${pkgdir}/usr/share/man/man1" install
}
