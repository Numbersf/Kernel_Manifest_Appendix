# Kernel_Manifest_Appendix
 
这是一个附加构建清单，它将覆盖一加天玑、真我的大部分机型，持续维护更新中....
如果有问题请及时反馈
 
天玑机型移花接木:
```
只需要kernel和vendor(kernel_modules_and_devicetree)两个仓库
修改例:
<project remote="origin" name="android_kernel_XXXXX_mtXXXX" path="kernel-这里填写内核版本" revision="XXXX">
                        ↓↓↓
    <linkfile dest="kernel/kernel-6.1" src="."/>
                        ↑↑↑
        将下方路径替换到上面
    <linkfile dest="kernel_platform/common" src="."/>
</project>
<project remote="origin" name="android_kernel_modules_and_devicetree_oneplus_mtXXXX" path="./" revision="XXXX"/>
```

README:
```
./kernel_platform/oplus/build/oplus_build_kernel.sh abc gki
 
abc:CPU代号，天玑机型请填写unknown
```