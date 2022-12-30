pkgname=tree
pkgver=2.1.0
pkgrel=1
pkgdesc="A directory listing program displaying a depth indented list of files"
arch=('x86_64')
url="http://mama.indstate.edu/users/ice/tree/"
license=('GPL')
depends=('glibc')
source=("http://mama.indstate.edu/users/ice/${pkgname}/src/${pkgname}-${pkgver}.tgz")
sha256sums=('0160c535bff2b0dc6a830b9944e981e3427380f63e748da96ced7071faebabf6')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make prefix="${pkgdir}/usr" MANDIR="${pkgdir}/usr/share/man/man1" install
}
