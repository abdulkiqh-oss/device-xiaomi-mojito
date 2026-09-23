# Reference: <https://postmarketos.org/devicepkg>
pkgname=device-xiaomi-mojito
pkgdesc="Xiaomi Redmi Note 10"
pkgver=4.14.190
pkgrel=3
url="https://postmarketos.org"
license="MIT"
arch="aarch64"
options="!check !archcheck"
depends="
	linux-xiaomi-mojito
	mkbootimg
	postmarketos-base
"
makedepends="devicepkg-dev"
source="
	deviceinfo
	modules-initfs
"

build() {
	devicepkg_build $startdir $pkgname
}

package() {
	devicepkg_package $startdir $pkgname
}

sha512sums="330ac56e7681fc00ab53cef0cc259ff0236918394ec9cef29b8af4b6afdeea39fdee8ba40d486009d373395ed25127867aa12490cea9a7820d22058e03cbdf78  deviceinfo


"
