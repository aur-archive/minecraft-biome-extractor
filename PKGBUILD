# Maintainer: ssc <chasessc@gmail.com>
pkgname=minecraft-biome-extractor
pkgver=0.9
pkgrel=2
pkgdesc="MBE is a cross-platform java program that taps into the biome generation code of Minecraft and outputs the color location on the "grasscolor.png" or "foliagecolor.png" for each block of a given map."
arch=('any')
url="http://www.minecraftforum.net/topic/76063-minecraft-biome-extractor-add-biome-support-to-your-mapper/"
license=('MIT')
groups=()
depends=('java-runtime>=5' 'bash')
makedepends=()
checkdepends=()
optdepends=('x-server')
provides=()
conflicts=()
replaces=()
backup=()
options=()
install="$pkgname.install"
changelog=
source=('http://dl.dropbox.com/u/107712/MCMap/Minecraft-Biome-Extractor-v090.zip' 'minecraft-biome-extractor.sh')
noextract=()
md5sums=('cff388ea201e7a90c82d5fcbb9be4af0'
         'f79e5f48da8e174e4c31a4bf912ea4b7')

package() {
  cd "$srcdir/Minecraft Biome Extractor"
  mkdir -p "$pkgdir/opt/minecraft-biome-extractor"
  mkdir -p "$pkgdir/usr/bin"
  cp "MinecraftBiomeExtractor.jar" "$pkgdir/opt/minecraft-biome-extractor"
  install -m 755 -T "$srcdir/minecraft-biome-extractor.sh" "$pkgdir/usr/bin/minecraft-biome-extractor"
}

# vim:set ts=2 sw=2 et:
