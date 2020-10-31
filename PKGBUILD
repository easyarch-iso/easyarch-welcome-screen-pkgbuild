pkgname=easyarch-welcome-screen
pkgver=2.1.1
pkgrel=1
pkgdesc="EasyArch Welcome Screen Application"
arch=('any')
url=https://github.com/easyarch-iso
source=("$pkgname-$pkgver::git+$url/easyarch-welcome-screen.git")
depends=(
    'gtk3'
    'xorg-xrandr'
    'python-gobject'
)
makedepends=(
    'make'
)
sha256sums=('SKIP')
options=(!strip)
package() {
    cd $srcdir/$pkgname-$pkgver/
    make DESTDIR="$pkgdir" install
}
