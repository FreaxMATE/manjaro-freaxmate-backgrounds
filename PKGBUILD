# Maintainer: Konstantin Unruh <freaxmate@protonmail.com>

pkgname=manjaro-freaxmate-backgrounds
pkgver=20211210
pkgrel=1
pkgdesc="FreaxMATE backgrounds."
arch=('any')
url="https://github.com/FreaxMATE/$pkgname"
license=('GPL3')
depends=('mate-screensaver')
makedepends=()
source=('git+https://github.com/FreaxMATE/manjaro-freaxmate-backgrounds.git')
sha512sums=('SKIP')

pkgver() {
    date +%Y%m%d
}

package() {
  cd "$pkgname"
  install -d $pkgdir/usr/share/backgrounds
  cp -r freaxmate-backgrounds $pkgdir/usr/share/backgrounds
  install -d $pkgdir/usr/share/mate-background-properties
  cp -r manjaro-freaxmate.xml $pkgdir/usr/share/mate-background-properties
}

