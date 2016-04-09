# Maintainer: Xin-Xin Wang <xin-xinw@musiclifephilosophy.com>
pkgname=bash-tools
pkgver=0.0.1
pkgrel=1
pkgdesc="Some tools I made"
url="https://github.com/xinxinw1/bash-tools"
license=('GPL')
arch=('any')

package() {
  # Creating directories
  find . -type d -print0 | xargs -0 -I % mkdir -p "$pkgdir/%"
  
  # Installing binaries
  find usr/bin -type f -print0 | xargs -0 -I % install -m 755 "%" "$pkgdir/%"
  
  # Installing other files
  find . -not \( -path "./usr/bin" -prune \) -type f -print0 | xargs -0 -I % install -m 644 "%" "$pkgdir/%"
}
