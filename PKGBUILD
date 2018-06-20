pkgname=neofetch
pkgver=5.0.0
pkgrel=1
pkgdesc="A CLI system information tool written in BASH that supports displaying images."
arch=('x86_64')
url="https://github.com/dylanaraps/${pkgname}"
license=('MIT')
depends=('bash')
source=("https://github.com/dylanaraps/${pkgname}/archive/${pkgver}.tar.gz")
md5sums=('807c41694ff5b861e4233eb71d507be9')

package() {
  cd "${srcdir}/${pkgname}-${pkgver}/"
  make DESTDIR="$pkgdir" install
  install -D -m644 LICENSE.md "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE.md"
}
