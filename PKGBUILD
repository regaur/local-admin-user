# Maintainer: Jan Boelsche <jan@lagomorph.de>

pkgname='local-admin-user'
pkgver=1.0
pkgrel=3
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

sha256sums=(
  '46c43f103be8f3d9294158ced51a89aa9d5a0215edd1e36584e92817a947d0e7'
  '554807de544674eacbd7a56aad43296ff7ca4c0e56a5141436b81f9795fc73cf'
)

package() {
  home=${pkgdir}/home/local-admin
	install -m 700 -d "${home}"
	install -m 644 -t "${home}" .tmux.conf .vimrc
}

	
