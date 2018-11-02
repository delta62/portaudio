# Maintainer: Sam Noedel <sam.noedel@gmail.com>
pkgname=portaudio
pkgver=19.2016.10.30
pkgrel=1
pkgdesc="Portable Cross-platform Audio I/O"
arch=('any')
url="http://www.portaudio.com"
license=('MIT')
depends=()
makedepends=()
checkdepends=()
optdepends=()
replaces=()
options=()
source=("http://www.portaudio.com/archives/pa_stable_v190600_20161030.tgz")
md5sums=("4df8224e047529ca9ad42f0521bf81a8")

build() {
  cd "$pkgname"
  ./configure --prefix=/usr
  make
}

package() {
  cd "$pkgname"
  make DESTDIR="$pkgdir/" install
}
