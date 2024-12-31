# Maintainer: Stefan Zipproth <s.zipproth@ditana.org>

pkgname=ditana-config-bash
pkgver=1.002
pkgrel=1
pkgdesc="Ditana bash config"
arch=(any)
url="https://ditana.org"
license=('GPL-3.0-or-later AND custom:WTFPL AND ISC')
conflicts=()
depends=(ditana-config-shell bash starship)
makedepends=()
source=("file://${PWD}/.bashrc_ditana" "file://${PWD}/ditana-bash-setup.sh")
sha256sums=('SKIP' 'SKIP')

package() {
	install -D -m644 "$srcdir/.bashrc_ditana" "$pkgdir/etc/skel/.bashrc_ditana"
	install -D -m644 "$srcdir/ditana-bash-setup.sh" "$pkgdir/etc/profile.d/ditana-bash-setup.sh"
}
