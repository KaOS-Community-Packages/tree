pkgname=tree
pkgver=2.1.1
pkgrel=1
pkgdesc="A directory listing program displaying a depth indented list of files"
arch=('x86_64')
url="http://mama.indstate.edu/users/ice/tree/"
license=('GPL')
depends=('glibc')
source=("http://mama.indstate.edu/users/ice/${pkgname}/src/${pkgname}-${pkgver}.tgz")
sha256sums=('d3c3d55f403af7c76556546325aa1eca90b918cbaaf6d3ab60a49d8367ab90d5')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make prefix="${pkgdir}/usr" MANDIR="${pkgdir}/usr/share/man/man1" install
}
