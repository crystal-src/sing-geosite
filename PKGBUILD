# Maintainer: everyx <lunt.luo#gmail.com>

pkgname=sing-geosite
pkgver=20230725085751
pkgrel=1

pkgdesc='sing-geosite database'
arch=('any')
_repo="SagerNet/${pkgname}"
url="https://github.com/${_repo}"
license=('GPL3')

optdepends=('sing-box: The universal proxy platform')

source=("${pkgver}.geosite.db::${url}/releases/download/${pkgver}/geosite.db"
        "${pkgver}.LICENSE::https://raw.githubusercontent.com/${_repo}/${pkgver}/LICENSE")
sha256sums=('11d2392bae6d51acb7914dc387c52da2160dd49ecb500c2f7235bfe605dd08e2'
            '2f02b7486bcfa90d115c71a20437f3906b6fd5bef81c5dc0efd341399e89d0fd')

package() {
    install -Dm644 "${pkgver}.geosite.db" "${pkgdir}/usr/share/${pkgname}/geosite.db"
    install -Dm644 "${pkgver}.LICENSE"    "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
