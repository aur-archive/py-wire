pkgname=py-wire
pkgver=0.4
pkgrel=3
pkgdesc="Client that implements the Wired protocol, written in Python."
arch=(any)
url="http://sourceforge.net/projects/pywire"
license=("MIT")
source=("http://downloads.sourceforge.net/pywire/py-wire-$pkgver.tar.gz")
depends=(python2-tlslite python2-distribute)
makedepends=(python2)
optdepends=("wipy: GUI frontend")
md5sums=('e9528284b6f7dc59538e50648e85f63d')

build() {
  cd "$srcdir/py-wire-$pkgver"
  python2 setup.py install \
    --prefix=$pkgdir/usr
}

package() {
  install -Dm644 "$srcdir/py-wire-$pkgver/README" "$pkgdir/usr/share/licenses/$pkgname/README"
}
