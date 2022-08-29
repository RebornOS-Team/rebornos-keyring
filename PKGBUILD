# Based on the file created for Arch Linux by:
# Pierre Schmitz <pierre@archlinux.de>

# Maintainer : Keegan Milsten <rebornos@protonmail.com>
# Maintainer : Rafael Costa Rega <rcostarega@gmail.com>

pkgname=rebornos-keyring
pkgver=20220425
pkgrel=1
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
            'df8b9355348db576c18c72352fea8e66061fff8fb82a03b401dba102e0e9713c'
            '44962ec2e8bf3666bbda99e525676f7545af93148d7367ac4eb5d85009e0b525'
            '0d89102f0b5977810f2656651d82dd2db3c815e3162083f26bb5015b266b903f')

pkgver() {
    date +%Y%m%d
}

package() {
	cd "${srcdir}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}
