# Maintainer: dryes <joswiseman@gmail>
pkgname='beautifybash'
pkgver=1.0
pkgrel=2
pkgdesc='A beautifier for Bash shell scripts written in Python.'
url='http://www.arachnoid.com/python/beautify_bash_program.html'
arch=('any')
license=('GPL')
depends=('python')
source=('http://www.arachnoid.com/python/python_programs/beautify_bash.py')
md5sums=('c063cbbb1efe479e5251a90f08567c99')

package() {
  sed -i -r 's|(\#\!/usr/bin/)env python|\1python|g;s|\(else\)|\(el\(se\|if\)\)|g' beautify_bash.py
  install -D -m755 "${srcdir}/beautify_bash.py" "${pkgdir}/usr/bin/beautifybash"
}
