# Maintainer: Gerd Zschaler <gzschaler at googlemail dot com>
pkgname=summon-secrets
pkgver=0.8.2
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
sha256sums=('57e47674c52687db6e015915b8a2e3d58adcd624b4ba1a887b10a7395de6d8aa'
            '6a7b308793f65cae9abbc02e02339fb87f46b8cabef1a7bb9164501f941bc332')

package() {
  mkdir -p "$pkgdir"/usr/bin
  cp summon "$pkgdir"/usr/bin

  mkdir -p "$pkgdir"/usr/share/licenses/summon-secrets
  cp LICENSE "$pkgdir"/usr/share/licenses/summon-secrets
}
