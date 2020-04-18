# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Valentin Rusu <valentin.rusu@endava.com>
pkgname=insync
pkgver=3.1.3.40790
pkgrel=1
epoch=
pkgdesc="insync OneDrive client re-packaged for ArchLinux"
arch=('x86_64')
url="https://www.insynchq.com/downloads"
license=('custom:insync')
depends=()
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=(!strip)
install=
changelog=
source=("insync-3.1.3.40790-fc30.x86_64.rpm::https://d2t3ff60b2tol4.cloudfront.net/builds/insync-${pkgver}-fc30.x86_64.rpm")
noextract=()
md5sums=('9b1c003aa3b7debdb3dfe2589aa93601')

package() {
  msg2 "Moving stuff in place..."
	install -D -m755 usr/bin/insync "$pkgdir"/usr/bin/insync
  install -D -m755 -d usr/lib/insync "$pkgdir"/usr/lib/insync
  cp -R usr/lib/insync/* "$pkgdir"/usr/lib/insync
}
