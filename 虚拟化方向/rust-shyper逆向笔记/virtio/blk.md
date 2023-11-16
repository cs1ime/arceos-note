





注册磁盘设备的代码在 `src/vmm/init.rs:235` 

虚拟机通过mmio和宿主机通信

```rust
EmuDeviceTVirtioBlk => {
                emu_register_dev(
                    EmuDeviceTVirtioBlk,
                    vm.id(),
                    idx,
                    emu_dev.base_ipa,
                    emu_dev.length,
                    emu_virtio_mmio_handler,
                );
                if !emu_virtio_mmio_init(vm.clone(), idx, emu_dev.mediated) {
                    return false;
                }
            }
```





处理



```
emu_virtio_mmio_handler->mmio.notify_handler->virtio_blk_notify_handler
```



