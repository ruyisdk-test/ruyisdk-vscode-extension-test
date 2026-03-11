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
+ 插件版本：[0.1.2](https://github.com/ruyisdk/ruyisdk-vscode-extension/releases/tag/0.1.2)
+ RuyiSDK版本：[0.46.0](https://github.com/ruyisdk/ruyi/releases/tag/0.46.0)
## 测试结果

共 19 个测试用例，成功 17 个，失败 2 个。
|          测试用例          | 结果  |                                          备注                                          |
| :------------------------: | :----:| :----------------------------------------------------------------------------------------------------------: |
|       版本更新提示冲突     |  失败 |    ruyisdk多版本状态下会重复提示版本更新       |
|       sysroot配置失败     |  失败 |    交互式配置sysroot时Enter跳过配置sysroot    | 