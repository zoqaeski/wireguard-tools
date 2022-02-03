# Maintainer: Robbie Smith <zoqaeski AT gmail DOT com>

pkgname=wgcg-git
pkgver=0.1
pkgrel=1
pkgdesc="Shell script to control a long-running mpv from the command line."
arch=('any')
url="https://github.com/zoqaeski/mpvctl"
license=('MIT')
depends=('wireguard-tools' 'zsh' 'gnupg' 'qrencode' 'grepcidr')
source=('wgcg.zsh'
        'LICENSE'
        'README.md')
sha256sums=('SKIP'
            'SKIP'
            'SKIP')

package() {
  cd "$srcdir"
  install -Dm755 ${pkgname}.zsh              "$pkgdir/usr/bin/${pkgname}"
  install -Dm644 LICENSE                     "$pkgdir/usr/share/licenses/${pkgname}/LICENSE"
  install -Dm644 README.md                   "$pkgdir/usr/share/doc/${pkgname}/README"
}
