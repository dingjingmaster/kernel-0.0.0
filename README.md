# kernel-0.0.0

取赵炯老师的源码编译[http://oldlinux.org/Linux.old/bochs/linux-0.00-050613.zip](http://oldlinux.org/Linux.old/bochs/linux-0.00-050613.zip)

编译成功后会在 bochs 里交替输出 A 和 B，生成的 Image镜像中包含了操作系统引导部分`boot`和系统主体部分`system`。

## 问题
- [ ] 目前使用 `objcopy -O binary` 转换后的 head 文件太大，导致生成的最终 Image 太大，目前还想不到解决方法。**ELF文件转为纯二进制文件后，怎么去掉无用内容?**
