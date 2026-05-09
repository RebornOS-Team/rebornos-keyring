# Based on the file created for Arch Linux by:
# Pierre Schmitz <pierre@archlinux.de>

pkgname=rebornos-keyring
pkgver=20260509
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
b2sums=('35a0d29ad01f26701f128b2870ce72b92d03b2928fa11d55676bd83786e8806abfc47a07f00c273c0c0b5afd5cdd2975ca2d2d33fea9755415fb1443c1f39622'
        '37351e07c32c714bd8f3403d4f01701c1bc04c0bf6cef8056ddb0f42ed4e4dcccf141ab52a397baa0ae08322906cece54f1ec5398001a34a81de2d2fd8fa2d34'
        '45d596aa3e825f42aceeeffd96c5dad1c6965b53f47a64d15f53b83674055c98796c1ca48fb387704d2a53b72402e4c8ec89758f96ddd157026267ed8ffc52f7'
        'ec332d5020d26b43521d97e47882dbd8b6e16c4e07862fbca5463b1f0d7153fb15cfca65b7377f995cc891419b816597d78addb834fda59f8d12c85b5f5a02ba')

pkgver() {
    date +%Y%m%d
}

package() {
    cd "${srcdir}"
    make PREFIX=/usr DESTDIR=${pkgdir} install
}
