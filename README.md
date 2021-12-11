# libtree

A tool that:
- :deciduous_tree: turns `ldd` into a tree
- :point_up: explains how shared libraries are found or why they cannot be located

![Screenshot of libtree](doc/screenshot.png)

## Building from sources

`libtree` requires a C compiler that understands c99

```
git clone https://github.com/haampie/libtree.git
cd libtree
make # recommended: CFLAGS="-static"
```

<details>
<summary>Or use the following unsafe quick install instructions</summary>
```
curl -Lfs https://raw.githubusercontent.com/haampie/libtree-in-c/master/libtree.c | cc -o libtree -x c - -std=c99 -D_FILE_OFFSET_BITS=64
```
</details>


