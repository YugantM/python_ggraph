pkgname=python-ggraph
pkgver=1.1
pkgrel=1
pkgdesc="topological sorting"
arch=("any")
makedepends=('python' 'python-setuptools')
url="https://github.com/YugantM/ggraph"
_dir="ggraph"
source=("${_dir}"::"git+https://github.com/yugantm/ggraph.git")
md5sums=('SKIP')

build() {
  cd "${srcdir}/${_dir}" 
  python setup.py build

}

package() {
  cd "${_dir}"
  python setup.py install --root="$pkgdir/" --optimize=1 --skip-build
}