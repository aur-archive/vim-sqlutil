# Maintainer: Zsolt Udvari <udvzsolt gmail com>
# Contributor: Nicholas Ring <nring8 gmail com>
pkgname=vim-sqlutil
pkgver=7.00
_scriptid=19113
pkgrel=1
pkgdesc="Formatting, generate - columns lists, procedures for databases"
arch=(any)
url="http://www.vim.org/scripts/script.php?script_id=492"
license=('custom')
depends=(vim vim-align)
groups=('vim-plugins')
install=vimdoc.install
source=(${pkgname}-${pkgver}.zip::http://www.vim.org/scripts/download_script.php?src_id=${_scriptid}
        license.txt)
md5sums=('453e4a74189748abbdaf0443101282b0'
         'efbd5986e691ce8c876fb86e8f5961ea')

build() {
    install -d ${pkgdir}/usr/share/vim/vimfiles/{autoload,doc,plugin}
    install -Dm644 ${srcdir}/doc/* ${pkgdir}/usr/share/vim/vimfiles/doc/ || return 1
    install -Dm644 ${srcdir}/plugin/* ${pkgdir}/usr/share/vim/vimfiles/plugin/ || return 1
    install -Dm644 ${srcdir}/autoload/* ${pkgdir}/usr/share/vim/vimfiles/autoload/ || return 1
    install -Dm644 ${srcdir}/license.txt ${pkgdir}/usr/share/licenses/${pkgname}/license.txt
}

