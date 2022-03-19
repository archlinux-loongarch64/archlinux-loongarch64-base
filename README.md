# archlinux-loongarch64-base
archlinux的loongarch64-bootstrap版本(为了可以迅速迭代跟进上游工具链，此项目只滚动base-devel包组)，基础工具链源码取自https://github.com/loongson 下的linux/gcc/glibc/binutils ，使用上游社区开源版本构建的新世界distro，运行在LoongArch平台。

### v0.2: archlinux-bootstrap-2022.03.18-loongarch64.tar.gz 
### sha256sum: a736ef2036ffad0b0103623c1124352231de60b255639ec7647ef0070ed66e94

* Fixed some software path issues

| package | branch | commit hash | url |
| ---- | ---- | ---- | ---- |
| binutils | upstream_v3.1 | f51838f4b4e0153acdf4a9849c17675775577cda | https://github.com/loongson/binutils-gdb.git |
| gcc | loongarch_upstream_v6.3 | 78c693aa2d833bfa27907141ba8bf93123b45567 | https://github.com/loongson/gcc.git |
| glibc | loongarch_2_35_dev_v2.2 | 74492b6d4613976aff5a9091a93d6ed4407d70a9 | https://github.com/loongson/glibc.git |
| linux | loongarch-next | 3643df5f058aacf69ac4121f6882500e843b7a34 | https://github.com/loongson/linux.git |
| systemd | dev-loongarch | 350489abb1c9ce4e43dab54b7af7d1a1bfbfb3b8 | https://github.com/loongarch64/systemd.git |
| libffi | loongarch-3_4_2 | 70602040e7a319ad4131aad422d59a493bc65f18 | https://github.com/loongson/libffi.git |
| libseccomp | dev-main | 5b4ba10fd1a9ad5baa85ebecafd36c401a030788 |https://github.com/loongarch64/libseccomp.git |

* A total of 114 software packages have been preinstalled

```
pacman -Q gcc binutils glibc linux-api-headers
gcc 12.0.1-3
binutils 2.37-3
glibc 2.35-2
linux-api-headers 5.17.0_rc1-1
```


