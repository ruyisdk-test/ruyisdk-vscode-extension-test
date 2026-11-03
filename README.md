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
+ 插件版本：[0.1.8-beta.1](https://github.com/ruyisdk/ruyisdk-vscode-extension/releases/tag/0.1.7-beta.1)
+ RuyiSDK版本：[0.53.0](https://github.com/ruyisdk/ruyi/releases/tag/0.53.0-beta.20260917)
## 测试结果

共 42 个测试用例，成功 38 个，失败 4 个。
|          测试用例          | 结果  |                                          备注                                          |
| :------------------------: | :----:| :----------------------------------------------------------------------------------------------------------:
|wlink不可见|失败 ||
|下载进度显示的软件包大小偏小（单位进制不一致）|失败||
|过低的如意版本时显示提示|失败|重复ruyi前缀|
|搜索有结果时仍提示未找到结果|失败||

