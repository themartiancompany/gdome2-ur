# SPDX-License-Identifier: AGPL-3.0
# 
# Maintainer: Truocolo <truocolo@aol.com>
# Maintainer: Pellegrino Prevete <pellegrinoprevete@gmail.com>

pkgname=gdome2
pkgver=0.8.1
pkgrel=1
pkgdesc="DOM level2 library for accessing XML files"
arch=(
  'any'
)
url="http://${pkgname}.cs.unibo.it"
license=(
  LGPL
)
depends=(
)
makedepends=()
source=(
  "${url}/tarball/${pkgname}-${pkgver}.tar.gz"
)
sha512sums=(
  '40d9cb9ade2db3c7a196ac30cf8d9f5b48da4990250c14a53db53280ee76870b9247e973e2f2da523807faed3333d7c0f854f9546860ffbda251c12f6d404da7'
)

build() {
  cd \
    "${pkgname}-${pkgver}"
  ./configure \
    --prefix=/usr
  make
}

package() {
  DESTDIR="$pkgdir" \
  make \
    install
}

# vim: ft=sh syn=sh et
