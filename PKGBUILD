pkgname=aszswaz-fonts
pkgver=1.0.2
pkgrel=1
pkgdesc='从网上收集的字体'
arch=('x86_64')
url=https://github.com/aszswaz/fonts
depends=(ttf-jetbrains-mono)

package() {
    # 切换到 PKGBUILD 文件所在目录，默认是 ${srcdir}：$(pwd)/src 目录
    cd ${startdir}
    install -dm 755 "${pkgdir}/usr/share/fonts/TTF"

    for font_file in *.ttf; do
        install -m 644 "$font_file" "${pkgdir}/usr/share/fonts/TTF/${font_file}"
    done

    for font_file in *.TTC; do
        install -m 644 "$font_file" "${pkgdir}/usr/share/fonts/TTF/${font_file}"
    done

    for font_file in *.ttc; do
        install -m 644 "$font_file" "${pkgdir}/usr/share/fonts/TTF/${font_file}"
    done
}
