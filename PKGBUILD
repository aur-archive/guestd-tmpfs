# Maintainer: Szabó Bence <szbence ät gmail d0t com>
pkgname=guestd-tmpfs
pkgver=0.1
pkgrel=1
pkgdesc="A simple daemon to create a guest account that automatically resets settings on shutdown using tmpfs."
arch=('any')
url="https://bbs.archlinux.org/viewtopic.php?pid=1029171"
license=('GPL')
depends=('coreutils')
conflicts=('guestd')
makedepends=('pkgconfig' 'coreutils')
install=$pkgname.install
source=($pkgname)
md5sums=('0b3940f9cb518681fa65c8dad966b3f9')

build()
{
  mkdir -p $pkgdir/etc/rc.d $pkgdir/home/{guest,guest-permanent}
  touch $pkgdir/home/guest-permanent/.keep
  cp $srcdir/guestd-tmpfs $pkgdir/etc/rc.d/guestd-tmpfs
}
