# make install
Exe install at build/bin/Demo

# rpm -ivh Demo.rpm
Exe install /usr/bin/Demo

# build.sh
rm -rf build
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=`pwd` ..
make
make install
make package
