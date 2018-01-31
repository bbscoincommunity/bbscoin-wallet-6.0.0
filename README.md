## OSX
```
brew install qt5
mkdir build && cd build
cmake .. -DCMAKE_BUILD_TYPE=Release -DCMAKE_PREFIX_PATH=/usr/local/Cellar/qt/5.10.0_1
make
```

## Ubuntu
```
ln -s ../bbscoin/ cryptonote
mkdir build && cd build
cmake ..
make
```

## Windows

You should compile the BBSCoin dynamic libs without rocksdb first, comment "add_subdirectory(tests)" line in bbscoin/CMakeLists.txt, and compile the packages/rocksdb-rocksdb-4.11.2.zip dynamic libs.
Then copy these files to the libs dir.

Finally, use CMake and VS compile this project.


