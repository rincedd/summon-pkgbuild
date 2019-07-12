# Maintainer: Gerd Zschaler <gzschaler at googlemail dot com>
pkgname=summon-secrets
pkgver=0.7.0
pkgrel=1
pkgdesc="Summon: a comand-line tool to provide secrets as environment variables"
arch=('x86_64')
url="https://cyberark.github.io/summon"
license=('MIT')
depends=()
makedepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
source=("${pkgname}-${pkgver}.tar.gz::https://github.com/cyberark/summon/releases/download/v${pkgver}/summon-linux-amd64.tar.gz"
"LICENSE::https://raw.githubusercontent.com/cyberark/summon/v${pkgver}/LICENSE"
)
noextract=()
sha256sums=('bf25218a3aa9b14a85282e95ec3607efef722d3ed3989d0373b378245bf54dbc'
            '6a7b308793f65cae9abbc02e02339fb87f46b8cabef1a7bb9164501f941bc332')

package() {
  mkdir -p "$pkgdir"/usr/bin
  cp summon "$pkgdir"/usr/bin

  mkdir -p "$pkgdir"/usr/share/licenses/summon-secrets
  cp LICENSE "$pkgdir"/usr/share/licenses/summon-secrets
}
