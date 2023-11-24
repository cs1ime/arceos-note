注释掉 `user/c/Cmakelist.txt` 中的

```
set(CMAKE_OBJDUMP           ${PREFIX}objdump)
set(CMAKE_RANLIB            ${PREFIX}ranlib)
```



编译：

```
cd kernel
make env    # for first time
make run ARCH=x86_64 LOG=warn
```

