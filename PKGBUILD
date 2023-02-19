# Based on the file created for Arch Linux by:
# Pierre Schmitz <pierre@archlinux.de>

# Maintainer : Panda <panda@rebornos.org>

pkgname=rebornos-keyring
pkgver=20230219
pkgrel=1
pkgdesc='RebornOS PGP keyring'
arch=('any')
url='https://github.com/RebornOS-Developers/rebornos-keyring'
license=('GPL')
install="${pkgname}.install"
source=('Makefile'
        'rebornos.gpg'
        'rebornos-revoked'
        'rebornos-trusted')
sha256sums=('947b8c2adb7bf76150f9bb686feb2135ecbbb57d0df7dc5a5a6ccfe0399e3a17'
            '1d828de001b5ce01033a06a9b6790f977a4ff002fc74bde0188b6ce12ad71a11'
            'd3a21399e86c20796ddafc55b1916674c415b1d935937c129b3eb62ba1fb56aa'
            '0e8fb55658872f3e3c78e5e4bb076972dd1a8775e42051155eaf34deaebc5836')

pkgver() {
    date +%Y%m%d
}

package() {
	cd "${srcdir}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}
