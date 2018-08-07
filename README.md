# SentencePiece

## Installation

### Build and Install SentencePiece
```
export THIRDPARTY=/export/home/autotest/3rdParty/linux/ubuntu-14.04/gcc-4.8.2/c++11/64/release-12
export PROTOBUF=$THIRDPARTY/protobuf/2.6.1
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$THIRDPARTY/protobuf/2.6.1/lib

mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=/export/home/zhang/projects/_bin/sentencepiece \
-DPROTOBUF_LIBRARY="$PROTOBUF/lib" \
-DPROTOBUF_INCLUDE_DIR="$PROTOBUF/include" \
-DPROTOBUF_PROTOC_EXECUTABLE="$PROTOBUF/bin/protoc" \
-DTCMALLOC_LIB="$THIRDPARTY/gperftools/2.5/lib" \
..

make
make install
```


