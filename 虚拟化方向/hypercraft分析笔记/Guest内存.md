



源码路径`apps/hv/src/x64.rs`下的全局变量  `GUEST_PHYS_MEMORY` 保存了Guest的所有物理内存，可以通过访问这个全局变量来实现以虚拟地址的形式访问Guest的所有物理内存

`setup_gpm` 函数的作用是设置并映射Guest内存范围



