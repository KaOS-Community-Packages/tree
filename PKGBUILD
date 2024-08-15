pkgname=tree
pkgver=2.1.3
pkgrel=1
pkgdesc="A directory listing program displaying a depth indented list of files"
arch=('x86_64')
url="http://oldmanprogrammer.net/source.php?dir=projects/tree"
license=('GPL')
depends=('glibc')
source=("https://github.com/Old-Man-Programmer/${pkgname}/archive/refs/tags/${pkgver}.tar.gz")
sha256sums=('3ffe2c8bb21194b088ad1e723f0cf340dd434453c5ff9af6a38e0d47e0c2723b')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make prefix="${pkgdir}/usr" MANDIR="${pkgdir}/usr/share/man/man1" install
}
