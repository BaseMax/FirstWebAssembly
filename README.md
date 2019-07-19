# First Web Assembly

WebAssembly (abbreviated Wasm) is a binary instruction format for a stack-based virtual machine. Wasm is designed as a portable target for compilation of high-level languages like C/C++/Rust, enabling deployment on the web for client and server applications.

# WASM

WebAssembly is an open standard that defines a portable binary code format for executable programs, and a corresponding textual assembly language, as well as interfaces for facilitating interactions between such programs and their host environment.


## Short Info

- **Filename extensions:** `.wat`, `.wasm`
- **First appeared:** March 2017; 2 years ago
- **License:** Apache License 2.0
- **Typing discipline:** Static
- **Designed by:** World Wide Web Consortium
- **Developer:** W3C; Mozilla; Microsoft; Google; Apple

## Install

$ git clone https://github.com/emscripten-core/emsdk.git 

$ cd emsdk/

$ ls
```
bin                           emsdk_env.fish              LICENSE
Dockerfile                    emsdk_env.ps1               python_selector
emcmdprompt.bat               emsdk_env.sh                README.md
emscripten-releases-tags.txt  emsdk_manifest.json         test.py
emsdk                         emsdk.ps1                   test.sh
emsdk.bat                     legacy-binaryen-tags.txt
emsdk_env.bat                 legacy-emscripten-tags.txt
```

$ ./emsdk install latest
```
Fetching emscripten-releases repository...
Cloning into '/home/max/emsdk/releases'...
remote: Total 2564 (delta 747), reused 2564 (delta 747)
Receiving objects: 100% (2564/2564), 1.25 MiB | 662.00 KiB/s, done.
Resolving deltas: 100% (747/747), done.
Fetching latest changes to the branch 'master' for '/home/max/emsdk/releases'...
Already up to date.
Successfully updated and checked out branch 'master' on repository '/home/max/emsdk/releases'
Current repository version: "Fri, 19 Jul 2019 05:41:08 +0000 d2967ba63d9c00c31b31f59702beba400921c7ca"
Fetching all precompiled tagged releases..
Downloading: /home/max/emsdk/llvm-tags-32bit.txt from https://s3.amazonaws.com/mozilla-games/emscripten/packages/llvm/tag/linux_32bit/index.txt
Downloading: /home/max/emsdk/llvm-tags-64bit.txt from https://s3.amazonaws.com/mozilla-games/emscripten/packages/llvm/tag/linux_64bit/index.txt, 2379 Bytes
Installing SDK 'sdk-releases-fastcomp-f42b12c45fd3f4c20de1321402fbc28f8fd21df1-64bit'..
Installing tool 'releases-fastcomp-f42b12c45fd3f4c20de1321402fbc28f8fd21df1-64bit'..
Downloading: /home/max/emsdk/zips/f42b12c45fd3f4c20de1321402fbc28f8fd21df1-wasm-binaries.tbz2 from https://storage.googleapis.com/webassembly/emscripten-releases-builds/linux/f42b12c45fd3f4c20de1321402fbc28f8fd21df1/wasm-binaries.tbz2, 166664114 Bytes
Unpacking '/home/max/emsdk/zips/f42b12c45fd3f4c20de1321402fbc28f8fd21df1-wasm-binaries.tbz2' to '/home/max/emsdk/fastcomp'
Done installing tool 'releases-fastcomp-f42b12c45fd3f4c20de1321402fbc28f8fd21df1-64bit'.
Installing tool 'node-8.9.1-64bit'..
Downloading: /home/max/emsdk/zips/node-v8.9.1-linux-x64.tar.xz from https://storage.googleapis.com/webassembly/emscripten-releases-builds/deps/node-v8.9.1-linux-x64.tar.xz, 11387108 Bytes
Unpacking '/home/max/emsdk/zips/node-v8.9.1-linux-x64.tar.xz' to '/home/max/emsdk/node/8.9.1_64bit'
Done installing tool 'node-8.9.1-64bit'.
Done installing SDK 'sdk-releases-fastcomp-f42b12c45fd3f4c20de1321402fbc28f8fd21df1-64bit'.
```
$ ./emsdk activate latest

[Read more](https://webassembly.org/getting-started/developers-guide/)
