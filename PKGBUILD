# Maintainer: Doridian <archlinux at doridian dot net>

pkgname=foxdenaur-keyring
pkgver=20250819
pkgrel=1
pkgdesc="FoxDen AUR keyring"
arch=(any)
url="https://foxden.network"
license=('GPL-3.0-or-later')
groups=(foxdenaur)
install=$pkgname.install
source=("foxdenaur.gpg"
        "foxdenaur-revoked"
        "foxdenaur-trusted"
        "$install")

b2sums=('8be5700c6d8364cfaecb575eb2d68ddd6193bddd85d89d25b86d2ec6ebabe30325158738042a5e105b553ed77681f263daca25f784ef841d87ed8f0a46eab949'
        '786a02f742015903c6c6fd852552d272912f4740e15847618a86e217f71f5419d25e1031afee585313896444934eb04b903a685b1448b755d56f701afe9be2ce'
        '1a07768d3d4409cb403ff812229599d512e40e24857b3391ce6433b31756f7070676cb1c3a85f1f5563393af4d2386509eccd37a89bc81f518e8ef09ab3221a8'
        'cf8554166a4831b0bab6a006d38f42994114f587dedafa23d700a8d36fe04495d5281fe7ed69ada317b6ceb5d88294d0e7d167fde7f71de99cac8cf32e5aa092')

package() {
    install -D -m0644 -t "${pkgdir}"/usr/share/pacman/keyrings/ 'foxdenaur'{.gpg,-trusted,-revoked}
}
