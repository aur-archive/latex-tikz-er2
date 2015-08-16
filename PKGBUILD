# Contributor: Pascal Wittmann <mail@pascal-wittmann.de>
# Pull requests are welcome: https://github.com/pSub/pkgbuilds
pkgname=latex-tikz-er2
pkgver=0.0
pkgrel=5
pkgdesc="A LaTeX Package for Drawing Entity-Relationship Diagrams based on Tikz"
arch=('any')
url="https://bitbucket.org/pavel_calado/tikz-er2/wiki/Home"
license=('CC Attribution 2.5 Generic License.')
depends=('texlive-core')
install=$pkgname.install
source=(https://bitbucket.org/pavel_calado/tikz-er2/raw/da9f9f7f169647cad6d91df7975400b1605ae67a/tikz-er2.sty)
md5sums=('9ae0d6eceb67b192d20a8504122cea38')

package() {
    install -dm755 "${pkgdir}/usr/share/texmf-dist/tex/latex/tikz-er2"
    cp tikz-er2.sty "${pkgdir}/usr/share/texmf-dist/tex/latex/tikz-er2"

    cd "${pkgdir}/usr/share/texmf-dist/tex/latex/"
    find . -type d -exec chmod 755 {} \;
    find . -type f -exec chmod 644 {} \;
}
