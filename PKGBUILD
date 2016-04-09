# Maintainer: Xin-Xin Wang <xin-xinw@musiclifephilosophy.com>
pkgname=bash-tools
pkgver=0.0.1
pkgrel=1
pkgdesc="Some tools I made"
url="https://github.com/xinxinw1/bash-tools"
license=('GPL')
arch=('any')

package() {
  mkdir -p "$pkgdir/usr/bin/"
  
  for f in *; do
    install -m 755 $f "$pkgdir/usr/bin/"
  done
}
