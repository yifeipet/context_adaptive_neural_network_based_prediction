# Tools for the two versions of HEVC/H.265 with the neural networks for intra prediction

This C++ code contains tools for integrating the neural networks for intra prediction
into HEVC/H.265.

## Compiling the tools
  * In Windows,
    * open the solution file "hevc\hm_common\c++\build\interface.sln"
	* choose the "Release" configuration and the "x64" platform
	* compile
  * In Linux,
    ```sh
    cd hevc/hm_common/c++/build/linux
    make
    cd ../../../../../
    ```

## Run the tests of the tools
The tests must be run from the root directory of the current project. This is because
many paths in these tests are defined relatively to this directory.

For instance, to test the function `extract_context_portions` in Windows,
```sh
hevc\hm_common\c++\bin\vc2015\x64\Release\interface.exe extract_context_portions
```
For instance, to test the function `extract_context_portions` in Linux,
```sh
./hevc/hm_common/c++/bin/executable extract_context_portions
```

