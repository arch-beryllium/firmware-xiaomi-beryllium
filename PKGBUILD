_hash=169925543541899dd9e471c50d9d3a8d1c376c073db1bcf2a9d698f1a3b8c490
pkgname=firmware-xiaomi-beryllium
pkgver=2
pkgrel=1
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
