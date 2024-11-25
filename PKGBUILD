pkgname=tree
pkgver=2.2.0
pkgrel=1
pkgdesc="A directory listing program displaying a depth indented list of files"
arch=('x86_64')
url="http://oldmanprogrammer.net/source.php?dir=projects/tree"
license=('GPL')
depends=('glibc')
source=("https://github.com/Old-Man-Programmer/${pkgname}/archive/refs/tags/${pkgver}.tar.gz")
sha256sums=('c4964b503d609e7146edd75566b978b1853e2cebee7c0342be230cbd84da326c')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make prefix="${pkgdir}/usr" MANDIR="${pkgdir}/usr/share/man/man1" install
}
