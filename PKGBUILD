# Maintainer: everyx <lunt.luo#gmail.com>

pkgname=sing-geosite
pkgver=20221201080109
pkgrel=1

pkgdesc='sing-geosite database'
arch=('any')
_repo="SagerNet/${pkgname}"
url="https://github.com/${_repo}"
license=('GPL3')

optdepends=('sing-box: The universal proxy platform')

source=("${pkgver}.geosite.db::${url}/releases/download/${pkgver}/geosite.db"
        "${pkgver}.LICENSE::https://raw.githubusercontent.com/${_repo}/${pkgver}/LICENSE")
sha256sums=('291bde9ac03a45c185f7b0b74562ad2fdfa312056ff9c78d40f44f49db46ae6b'
            '2f02b7486bcfa90d115c71a20437f3906b6fd5bef81c5dc0efd341399e89d0fd')

package() {
    install -Dm644 "${pkgver}.geosite.db" "${pkgdir}/usr/share/${pkgname}/geosite.db"
    install -Dm644 "${pkgver}.LICENSE"    "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
