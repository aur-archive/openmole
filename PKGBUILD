# Maintainer: Martin Potier <mpo+PKGBUILD@marvid.fr>
pkgname=openmole
pkgver=0.10.0
pkgrel=3
pkgdesc="A workflow engine designed to easily put processes in parallel."
arch=('i686' 'x86_64')
url="http://www.openmole.org"
license=('AGPLv3')
depends=('java-runtime')
optdepends=()
provides=("openmole")
conflicts=("openmole")
source=($pkgname-$pkgver.tgz::http://openmole.org/files/$pkgname-$pkgver-RC2.tgz openmole.sh)
md5sums=('5401f58ad639e7fb5bdb063b69fe3ac4'
         'b0e78d3c7e6053b1f968870965b38f85')

package() {
  cd "$srcdir/$pkgname"
  mkdir -p $pkgdir/opt/$pkgname

  cp -r * $pkgdir/opt/$pkgname
  install -Dm 755 ../openmole.sh $pkgdir/usr/bin/$pkgname
}
