# Contributor: Alexander Oleynichenko <alexvoleynichenko@gmail.com>
pkgname=materials_studio
pkgver=2017
pkgrel=1
epoch=
pkgdesc="BIOVIA Materials Studio"
arch=('x86_64')
url="http://www.3dsbiovia.com/products/collaborative-science/biovia-materials-studio/"
license=('custom')
groups=()
depends=('libsm')
makedepends=('perl')
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=('DS.Biovia.Materials.Studio.2017.Linux.iso'
        'msi_SSQ.lic')
noextract=()
md5sums=('SKIP'
         'SKIP')
validpgpkeys=()

_installdir="/opt/biovia/${pkgname}"

prepare() {
    chmod +w -R ${srcdir}
}

package() {
    "${srcdir}/install" --nonroot --installroot=${pkgdir}${_installdir} --lproot=${pkgdir}${_installdir} --user=$USER --group=$USER
}
