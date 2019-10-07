# Valgrind

## Overview
Valgrind is an undefined behavior checking tool, a function and memory profiler tool, a data-race detection tool and a leak checking tool. 

## Standard install via command-line
```
git clone --recursive https://github.com/manikamakam/Valgrind.git
cd <path to repository>
mkdir build
cd build
cmake ..
make
Run tests: ./test/cpp-test
Run program: ./app/shell-app

```
## Valgrind outputs

The following commands were run and the detected two bugs were fixed

1. valgrind ./app/shell-app
2. valgrind --tool=helgrind ./app/shell-app
3. valgrind --leak-check=full ./app/shell-app

The valgrind outputs before and after fixing the bugs are shown in separate text documents in the outputs folder. KCachegrind output is also attached in the same folder.
