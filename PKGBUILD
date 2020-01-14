# Maintainer: Felipe Morales <hel.sheep@gmail.com>
pkgname=neovim-gnome-terminal-wrapper
pkgver=2
pkgrel=14
pkgdesc="A wrapper for running neovim in a separate instance of gnome-terminal"
arch=(any)
url="http://github.com/fmoralesc/"
license=('GPL')
groups=()
depends=('python-dbus' 'neovim' 'gnome-terminal')
source=('neovim.desktop'
        'nvim-wrapper'
        'neovim.svg')
md5sums=('a2d9fa3e74a095cdc4c44629859a3f03'
         'b6a5da7372c8f165371b1560f96bb7a3'
         '2b271742492f200bcac78dbfe33caa3c')

package() {
  cd "$srcdir/"
  install -Dm755 nvim-wrapper "$pkgdir/usr/bin/nvim-wrapper"
  install -Dm644 neovim.desktop "$pkgdir/usr/share/applications/neovim.desktop"
  install -Dm644 neovim.svg "$pkgdir/usr/share/icons/neovim.svg"
}

# vim:set ts=2 sw=2 et:
