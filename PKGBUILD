# Maintainer: Jan Boelsche <jan@lagomorph.de>

pkgname='local-admin-user'
pkgver=1.1
pkgrel=1
pkgdesc='Creates a user called "local-admin", installs some dotfiles and set a random password'
packager='Jan Boelsche'
arch=('any')
license=('GPL')
groups=()
depends=()
makedepends=()
checkdepends=()
optdepends=()
install=${pkgname}.install
source=(.vimrc .tmux.conf )

sha256sums=('a8668316913ad6a3aa28c814d1cc65c6215574bf22010cbbac2ae3470f52478d'
            '554807de544674eacbd7a56aad43296ff7ca4c0e56a5141436b81f9795fc73cf')

package() {
  home=${pkgdir}/home/local-admin
	install -m 700 -d "${home}"
	install -m 644 -t "${home}" .tmux.conf .vimrc
}

	
