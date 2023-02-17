# Maintainer: aszswaz <aszswaz@163.com>

pkgname=aszswaz-fonts
pkgver=1.0.4
pkgrel=1
pkgdesc='从网上收集的字体'
arch=('x86_64')
url=https://github.com/aszswaz/fonts
depends=('adobe-source-han-sans-cn-fonts' 'ttf-jetbrains-mono-nerd')
groups=('aszswaz')

package() {
    ORIGINAL_IFS="$IFS"

    # 切换到 PKGBUILD 文件所在目录，默认是 ${srcdir}：$(pwd)/src 目录
    cd ${startdir}
    install -dm 755 "${pkgdir}/usr/share/fonts/TTF"

    IFS=$'\n'
    for font_file in $(find -iname '*.ttf' -or -iname '*.ttc' -type f); do
        install -m 644 -D "$font_file" "${pkgdir}/usr/share/fonts/TTF/${font_file}"
    done

    IFS="$ORIGINAL_IFS"
}
