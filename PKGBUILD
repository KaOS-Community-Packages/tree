pkgname=tree
pkgver=2.0.3
pkgrel=1
pkgdesc="A directory listing program displaying a depth indented list of files"
arch=('x86_64')
url="http://mama.indstate.edu/users/ice/tree/"
license=('GPL')
depends=('glibc')
source=("http://mama.indstate.edu/users/ice/${pkgname}/src/${pkgname}-${pkgver}.tgz")
sha256sums=('ba14e77b5f9dc7f8250c3f702ec5b6be2f93cd0fa87311bab3239676866a3b1d')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make prefix="${pkgdir}/usr" MANDIR="${pkgdir}/usr/share/man/man1" install
}
