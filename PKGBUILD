pkgname=firmware-xiaomi-beryllium
pkgver=0.1
pkgrel=1
pkgdesc='Linux firmware for Xiaomi Beryllium'
arch=(any)
url='https://gitlab.com/sdm845-mainline/firmware-xiaomi-beryllium'
provides=($pkgname-git)
conflicts=(linux-firmware $pkgname-git)
_commit=aad74c8d4f6fb5852a20bebdebb2979ee63ed775
source=("https://gitlab.com/sdm845-mainline/firmware-xiaomi-beryllium/-/archive/$_commit/firmware-xiaomi-beryllium-$_commit.tar.gz")
sha256sums=('c6d322e2ff2afb35e7b66acbf12ba35cfa96303ed49eeac858f2385be9241bdc')
options=('!strip')

package() {
  mkdir -p "$pkgdir"/usr/lib
  cp $srcdir/firmware-xiaomi-beryllium-$_commit/lib/firmware "$pkgdir"/usr/lib -r
}
