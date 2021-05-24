_hash=f8143250287452ab4a60fdbc00d84549f544012835a781128d3c3504880db93a
pkgname=firmware-xiaomi-beryllium
pkgver=1
pkgrel=2
pkgdesc='Linux firmware for Xiaomi Beryllium'
arch=(any)
url='https://github.com/arch-beryllium/firmware'
provides=($pkgname-git)
conflicts=(linux-firmware $pkgname-git)
source=("$_hash.tar.gz::https://github.com/arch-beryllium/firmware/releases/download/$_hash/firmware.tar.gz")
sha256sums=("$_hash")
options=('!strip')

package() {
  mkdir -p $pkgdir/usr
  cp $srcdir/lib $pkgdir/usr -r
}
