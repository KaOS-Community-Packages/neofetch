pkgname=neofetch
pkgver=6.0.0
pkgrel=1
pkgdesc="A CLI system information tool written in BASH that supports displaying images."
arch=('x86_64')
url="https://github.com/dylanaraps/${pkgname}"
license=('MIT')
depends=('bash')
source=("https://github.com/dylanaraps/${pkgname}/archive/${pkgver}.tar.gz")
md5sums=('53b8c8b0ca4b0cd01a27ac7773a5eefd')

package() {
  cd "${srcdir}/${pkgname}-${pkgver}/"
  make DESTDIR="$pkgdir" install
  install -D -m644 LICENSE.md "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE.md"
}
