_hash=6a606321317764b2eb7e0b4b21b698d16a89e22d3075d7f2ee5f0b0d38b3c014
pkgname=firmware-xiaomi-beryllium
pkgver=2
pkgrel=2
pkgdesc='Linux firmware for Xiaomi Beryllium'
arch=(any)
url='https://github.com/arch-beryllium/firmware'
provides=($pkgname-git)
conflicts=($pkgname-git)
depends=(linux-firmware)
source=("$_hash.tar.gz::https://github.com/arch-beryllium/firmware/releases/download/$_hash/firmware.tar.gz")
sha256sums=("$_hash")
options=('!strip')

package() {
  mkdir -p $pkgdir/usr
  cp $srcdir/lib $pkgdir/usr -r
}
