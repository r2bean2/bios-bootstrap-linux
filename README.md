frist, download the corect toolchain from musl.cc for your architecture (you can build your own, but these toolchains are known to work, and you can put the tar file anywere, i.e. its not linked agnst any of your files, and it comes with the headers you need)
download the busybox 1.38, replace the .config (hold contol+h to see invisable files) witht the file (shell script to autmate the replacment coming later) and run make CC=/path/to/exicutable/from/downloaded/toolchain/x86_64-linux-musl-cross/bin/x86_64-linux-musl-gcc -j$(nproc)
&& make install
