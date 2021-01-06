_pkgname=firmware-xiaomi-beryllium
pkgname=$_pkgname-git
pkgver=r7.g5dff7ac
pkgrel=2
pkgdesc='Linux firmware for Xiaomi Beryllium'
arch=(any)
url='https://gitlab.com/sdm845-mainline/firmware-xiaomi-beryllium.git'
provides=($_pkgname)
conflicts=(linux-firmware)
source=("git+https://gitlab.com/sdm845-mainline/firmware-xiaomi-beryllium.git")
sha256sums=('SKIP')

pkgver() {
  cd $_pkgname
  printf "r%s.g%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
  mkdir -p "$pkgdir"/usr/lib
  cd $_pkgname
  cp lib/firmware "$pkgdir"/usr/lib -r
}
