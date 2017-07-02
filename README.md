# travis test  
[![Build Status](https://travis-ci.org/mocabe/travis-test.svg?branch=master)](https://travis-ci.org/mocabe/travis-test) [![Build status](https://ci.appveyor.com/api/projects/status/xk6s17ksi03p6w6l/branch/master?svg=true)](https://ci.appveyor.com/project/mocabe/travis-test/branch/master)

## memo
### ```.travis.yml```
- To get latest clang, use ```dist: trusty``` and speficy ```llvm-toolchain-trusty``` for source.
    - same for latest g++. source is ```ubuntu-toolchain-r-test```.
- An easy way to multi-compiler test is using ```env: COMPILER=***``` to export variable ```$COMPILER```.
    - then add ```-DMAKE_CXX_COMPILER=$COMPILER``` option after ```cmake```.
### ```.appveyor.yml```
- need to config ```-C <config>``` to run ```ctest```  


