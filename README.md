# 针对RuyiSDK VSCode插件的测试

## 测试说明

以手动测试的方法，验证VSCode插件的核心功能与关键路径。

## 安装方法

- 从仓库页面下载最新构建的压缩包，解压获得 `ruyisdk-vscode-extension-<version>.vsix`
    - 在 VS Code 中执行 “Install from VSIX…”，确认安装成功
- 从Vscode Marketplace中搜索关键词，安装插件
## 环境配置

+ OS: Ubuntu 25.04 (Plucky Puffin)
+ cpu: 16 核
+ 内存：4G
+ 镜像：https://releases.ubuntu.com/25.04/ubuntu-25.04-desktop-amd64.iso
+ 插件版本：[0.1.6-beta.1](https://github.com/ruyisdk/ruyisdk-vscode-extension/releases/tag/0.1.6-beta.1)
+ RuyiSDK版本：[0.49.0](https://github.com/ruyisdk/ruyi/releases/tag/0.49.0)
## 测试结果

共 33 个测试用例，成功 27 个，失败 6 个。
|          测试用例          | 结果  |                                          备注                                          |
| :------------------------: | :----:| :----------------------------------------------------------------------------------------------------------: |
|i18n|失败|为新建的虚拟环境中包含sysroot中选择 选择软件包进入的列表中为英文|
|emulator排序意义不明|失败||
|最新版工具链排序问题|失败||
|ruyi package 切换镜像源时，需手动刷新当前的软件包状态|失败||
|ruyi存在多个镜像源时，存在软件包安装冲突（状态异常）|失败||
|版本切换过程中中英文切换不灵活|失败||


