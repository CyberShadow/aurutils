pkgname=aurutils-git
pkgver=r89.278f05b
pkgrel=1
pkgdesc='AUR helpers tools'
arch=('any')
url=https://github.com/AladW/aurutils
license=('ISC')
source=("git+$url")
depends=('pacman>=5.0')
makedepends=('git')
optdepends=('repose-git: aurbuild'
            'powerpill: aurbuild'
            'jshon: aurchain'
            'pacutils-git: aurqueue, aurbuild'
            'expac: aurqueue'
            'git: aurclone'
            'aria2: aursearch'
            'vifm: aurbob')

pkgver() {
    printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}    

package() {
    cd aurutils
    install -d "$pkgdir"/usr/bin
    install -m755 * "$pkgdir"/usr/bin
}

md5sums=('SKIP')
