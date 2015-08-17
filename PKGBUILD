# Maintainer: ammon117@gmail.com

pkgname=python2-npyscreen
pkgver=4.3.5
pkgrel=1
_libname=${pkgname/python2-/}
pkgdesc="This library provides a framework for developing console applications using Python and curses."
url="https://code.google.com/p/npyscreen/"
license=('BSD-3')
arch=('i686' 'x86_64' 'armv6h')
source=(http://pypi.python.org/packages/source/${_libname:0:1}/$_libname/$_libname-$pkgver.tar.gz)

build() {
	cd "$srcdir/$_libname-$pkgver"
	python2 setup.py build
}

package() {
	cd "$srcdir/$_libname-$pkgver"
	python2 setup.py install -O1 --skip-build --root="$pkgdir"
}

md5sums=('a2ce1f624eb9867b6802a86b43b475cc')

