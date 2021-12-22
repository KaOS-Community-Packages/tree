pkgname=tree
pkgver=2.0.0
pkgrel=1
pkgdesc="A directory listing program displaying a depth indented list of files"
arch=('x86_64')
url="http://mama.indstate.edu/users/ice/tree/"
license=('GPL')
depends=('glibc')
source=("http://mama.indstate.edu/users/ice/${pkgname}/src/${pkgname}-${pkgver}.tgz")
sha256sums=('782cd73179f65cfca7f29326f1511306e49e9b11d5b861daa57e13fd7262889f')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make prefix="${pkgdir}/usr" MANDIR="${pkgdir}/usr/share/man/man1" install
} 
