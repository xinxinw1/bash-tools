# Maintainer: Xin-Xin Wang <xin-xinw@musiclifephilosophy.com>
pkgname=bash-tools
pkgver=0.0.1
pkgrel=1
pkgdesc="Some tools I made"
url="https://github.com/xinxinw1/bash-tools"
license=('GPL')
arch=('any')

package() {
  # Installing binaries
  mkdir -p "$pkgdir/usr/bin/"
  for f in bin/*; do
    install -m 755 "$f" "$pkgdir/usr/bin/"
  done
  
  # Installing shares
  mkdir -p "$pkgdir/usr/share/bash-tools/"
  for f in share/*; do
    install -m 644 "$f" "$pkgdir/usr/share/bash-tools/"
  done
}
