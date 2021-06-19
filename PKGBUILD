# Based on the file created for Arch Linux by:
# Pierre Schmitz <pierre@archlinux.de>

# Maintainer : Keegan Milsten <rebornos@protonmail.com>
# Maintainer : Rafael Costa Rega <rcostarega@gmail.com>

pkgname=rebornos-keyring
pkgver=20210512
pkgrel=1.2
pkgdesc='RebornOS PGP keyring'
arch=('any')
url='https://gitlab.com/rebornos-team/rebornos-special-system-files/rebornos-keyring'
license=('GPL')
install="${pkgname}.install"
source=('Makefile'
        'rebornos.gpg'
        'rebornos-revoked'
        'rebornos-trusted')
sha256sums=('947b8c2adb7bf76150f9bb686feb2135ecbbb57d0df7dc5a5a6ccfe0399e3a17'
            '2fc25886de5a124c592d67e54252c29eac073a1feb54de919c66183681799537'
            '44962ec2e8bf3666bbda99e525676f7545af93148d7367ac4eb5d85009e0b525'
            'b92fd8eca8d57f2142e6f987d90a5e3c69023c081b5974e3b7bee4968b5ff299')

pkgver() {
    date +%Y%m%d
}

package() {
	cd "${srcdir}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}
