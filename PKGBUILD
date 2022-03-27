pkgname=aszswaz-fonts
pkgver=1.0.0
pkgrel=1
pkgdesc='从网上收集的字体'
arch=('x86_64')
url=https://github.com/aszswaz/fonts

package() {
    # 切换到 PKGBUILD 文件所在目录，默认是 ${srcdir}：$(pwd)/src 目录
    cd ${startdir}
    install -dm 755 "${pkgdir}/usr/share/fonts/TTF"
    install -m 644 130-ss-Zhui-Guang-Shou-Xie-Ti.ttf "${pkgdir}/usr/share/fonts/TTF/130-ss-Zhui-Guang-Shou-Xie-Ti.ttf"
    install -m 644 JBHGXK.ttf "${pkgdir}/usr/share/fonts/TTF/JBHGXK.ttf"
}
