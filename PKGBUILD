# Based on the file created for Arch Linux by:
# Pierre Schmitz <pierre@archlinux.de>

pkgname=rebornos-keyring
pkgver=20230728
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
sha256sums=('1e4d3eb7f86f782b4598cbd1dd4879907fcaa216d06a821d64dced1fe2b20960'
    '94b23c1a9e24f920d6108f18ac81afdb438007bb5fadbfd691ac13a77e7588ac'
    '8c314e0e53fffccb7a6eca0c7608e6d3aef51621e0f71d48861452ddd3000003'
    '1ba9767a5b72d1766e0d1da276f94833596620a2f39077ce51bcd04683edbdfa')

pkgver() {
    date +%Y%m%d
}

package() {
    cd "${srcdir}"
    make PREFIX=/usr DESTDIR=${pkgdir} install
}
