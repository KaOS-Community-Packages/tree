pkgname=tree
pkgver=2.0.1
pkgrel=1
pkgdesc="A directory listing program displaying a depth indented list of files"
arch=('x86_64')
url="http://mama.indstate.edu/users/ice/tree/"
license=('GPL')
depends=('glibc')
source=("http://mama.indstate.edu/users/ice/${pkgname}/src/${pkgname}-${pkgver}.tgz")
sha256sums=('e3339c5a194cf6b4080f15ec59faa3679f02d5a793b2147912fbfcfb4cdf2239')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make prefix="${pkgdir}/usr" MANDIR="${pkgdir}/usr/share/man/man1" install
} 
