# Maintainer: kozec <kozec at kozec dot com>
# Based on minecraft package by Christophe Robin
pkgname=spoutcraft
pkgver=1.5.2.b2039
pkgrel=1
pkgdesc="Launcher and client-side mod for Minecraft"
arch=(i686 x86_64)
license=('custom')
url="http://www.spout.org/"
depends=('java-runtime' 'xorg-server-utils' 'openal')
source=(spoutcraft
	http://get.spout.org/Spoutcraft.jar
	spoutcraft.desktop spoutcraft.png)

build() {
	true
}

package() {
    cd "$srcdir" || return 1

    install -D -m755 "${srcdir}/spoutcraft"         "${pkgdir}/usr/bin/spoutcraft"
    install -D -m644 "${srcdir}/Spoutcraft.jar"     "${pkgdir}/usr/share/spoutcraft/Spoutcraft.jar"

    # Desktop launcher with icon
    install -D -m644 "${srcdir}/spoutcraft.desktop" "${pkgdir}/usr/share/applications/spoutcraft.desktop"
    install -D -m644 "${srcdir}/spoutcraft.png"     "${pkgdir}/usr/share/pixmaps/spoutcraft.png"
}

md5sums=('8e026f5581e72aeb8928d4ba30fd3488'
         'f2f45dd75fc7c2aa40dabfc593f1602e'
         '71f37490d1ec1ef74488ae18e235d230'
         '71170c397a5c110b7b80051d1339d69c')
