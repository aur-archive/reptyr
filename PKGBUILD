pkgname=reptyr
pkgver=0.4
pkgrel=1
pkgdesc="A tool for \"re-ptying\" programs"
arch=('i686' 'x86_64')
license=('BSD')
url="https://github.com/nelhage/reptyr"
depends=('openssl')
source=("$pkgname-$pkgver.tar.gz::https://github.com/nelhage/$pkgname/tarball/$pkgname-$pkgver")
md5sums=('4846a0b22c267a154853ce1409e823da')

build() {
	cd "$srcdir"/nelhage-$pkgname-*

	make
}

package() {
	cd "$srcdir"/nelhage-$pkgname-*

	make "DESTDIR=$pkgdir" "PREFIX=/usr" install
} 
