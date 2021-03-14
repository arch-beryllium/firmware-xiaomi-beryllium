pkgname=firmware-xiaomi-beryllium
pkgver=0.1
pkgrel=2
pkgdesc='Linux firmware for Xiaomi Beryllium'
arch=(any)
url='https://gitlab.com/sdm845-mainline/firmware-xiaomi-beryllium'
provides=($pkgname-git)
conflicts=(linux-firmware $pkgname-git)
_commit=aad74c8d4f6fb5852a20bebdebb2979ee63ed775
source=("https://gitlab.com/sdm845-mainline/firmware-xiaomi-beryllium/-/archive/$_commit/firmware-xiaomi-beryllium-$_commit.tar.gz"
        "git://git.kernel.org/pub/scm/linux/kernel/git/firmware/linux-firmware.git")
sha256sums=('c6d322e2ff2afb35e7b66acbf12ba35cfa96303ed49eeac858f2385be9241bdc'
            'SKIP')
options=('!strip')

package() {
  mkdir -p "$pkgdir"/usr/lib/firmware "$pkgdir"/usr/lib/firmware/qca

  cp $srcdir/firmware-xiaomi-beryllium-$_commit/lib/firmware "$pkgdir"/usr/lib -r

  cp $srcdir/linux-firmware/ath10k/WCN3990/hw1.0/firmware-5.bin "$pkgdir"/usr/lib/firmware/ath10k/WCN3990/hw1.0
  cp $srcdir/linux-firmware/qcom/a630_sqe.fw "$pkgdir"/usr/lib/firmware/qcom
  cp $srcdir/linux-firmware/qcom/a630_gmu.bin "$pkgdir"/usr/lib/firmware/qcom
  cp $srcdir/linux-firmware/qca/crbtfw21.tlv "$pkgdir"/usr/lib/firmware/qca
  cp $srcdir/linux-firmware/qca/crnv21.bin "$pkgdir"/usr/lib/firmware/qca
}
