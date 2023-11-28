# Based on the file created for Arch Linux by:
# Pierre Schmitz <pierre@archlinux.de>

pkgname=rebornos-keyring
pkgver=20231128
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
    'be2f4518b82bcc96e6b09e1dce02f6decb6a851efbca12391a5b8d9a679294e9d6a7c14d81834ce3a0f5cbb3eafda279f79dfa8bad583f7f7f31bfb4b0901cb5'
    '45d596aa3e825f42aceeeffd96c5dad1c6965b53f47a64d15f53b83674055c98796c1ca48fb387704d2a53b72402e4c8ec89758f96ddd157026267ed8ffc52f7'
    '7ba550c7311b81943869d7b42cedbe0aa68deba1cad7f53044aa3724be80a205d6e12adeab9cdcc15a06fe311d58a8331af64516e29affeb936f4371d9b356bd')

pkgver() {
    date +%Y%m%d
}

package() {
    cd "${srcdir}"
    make PREFIX=/usr DESTDIR=${pkgdir} install
}
