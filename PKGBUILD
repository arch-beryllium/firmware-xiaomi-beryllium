_hash=e3d05adb57894563e334159ae69e6b3f8b7eef7a24fae7d7cb316cb80604b48c
pkgname=firmware-xiaomi-beryllium
pkgver="$(echo $_hash | cut -c1-8)"
pkgrel=1
pkgdesc='Linux firmware for Xiaomi Beryllium'
arch=(any)
url='https://github.com/arch-beryllium/firmware'
provides=($pkgname-git)
conflicts=(linux-firmware $pkgname-git)
source=("https://github.com/arch-beryllium/firmware/releases/download/$_hash/firmware.tar.gz")
sha256sums=("$_hash")
options=('!strip')

package() {
  mkdir -p $pkgdir/usr
  cp $srcdir/lib $pkgdir/usr -r
}
