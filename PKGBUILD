
pkgname=python-spacy-language-detection
_pkgname=spacy-language-detection
pkgver=0.2.1
pkgrel=1 
url="https://files.pythonhosted.org/packages/60/48/f86fad67d6afc03cbfb50eb872fc401698108fc687cfdccfbfe562e79661/spacy-language-detection-0.2.1.tar.gz"
arch=('any')
license=('MIT')
depends=('python')
source=('https://files.pythonhosted.org/packages/60/48/f86fad67d6afc03cbfb50eb872fc401698108fc687cfdccfbfe562e79661/'$_pkgname'-'$pkgver'.tar.gz')
md5sums=('40c83f73ea02a0b22a2fc41a0e7be3ee')

build(){
	cd "$srcdir/$_pkgname-$pkgver"
	echo 'version='$pkgver >version.txt
	python setup.py build
}

package(){
  cd "$srcdir/$_pkgname-$pkgver"
  python setup.py install --root="$pkgdir" --optimize=1
}
