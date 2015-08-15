# Contributor: Testuser_01 <arch@nico-siebler.de>

pkgname=cryptcat
pkgver=1.2.1
pkgrel=2
pkgdesc="Cryptcat is a lightweight version of netcat with integrated transport encryption capabilities."
arch=('any')
url="http://sourceforge.net/projects/${pkgname}/"
license=('GPL')
depends=('glibc')
provides=('cryptcat')
source=("http://downloads.sourceforge.net/cryptcat/cryptcat-unix-${pkgver}.tar")
md5sums=('fc4afff350f3dd5e4fe51b0dd01a8e21')

build() {
  cd 'unix' || return 1
  make linux || return 1
  install -m755 -D "${pkgname}" "${pkgdir}/usr/bin/${pkgname}" || return 1
}
