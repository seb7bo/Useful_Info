# Useful_Info
Useful command for gdb,bash,linux,etc....

## LINUX

* Tree patterns for specific file

```console
tree -P "*.a" --prune
```

* search string in repos

```console
grep -r "adas_base_utils_if"
```

* max depth

```console
du -h --max-depth=1
```

* HDD Size

```console
df -h
```

## CMake

* Print variables of stuff

```cmake
message(PROJECT_SOURCE_DIR="${PROJECT_SOURCE_DIR}")
```

## GDB

* Show all sources of the binary

```console
info sources
```

* Show locals

```console
info locals
```

* Show file source

```console
list filename.c:1
```

* Set break point

```console
break src/utils/helpers.c:15
```

* Print pointer or variable

```console
set print pretty on
print *this
```

* conditional breakpoint 

```console
break main.cpp:43 if result == 0
```

* set variable value

```console
set variable <varname> = <value>

```

* info break points

Note: disable, enable and delete

```console
info breakpoints
```

### Optimization

```cpp
#pragma clang optimize off
```

## Gtest

Execute specific test

```console
./your_test_binary --gtest_filter=MyTestSuite.MySpecificTest
```
