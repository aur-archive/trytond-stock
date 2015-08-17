# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-stock
_pkgname=trytond_stock
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The stock module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-company>=3.4' 'trytond-currency>=3.4' 'trytond-party>=3.4' 'trytond-product>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("d90a01b5203183209e97481445311f54")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}