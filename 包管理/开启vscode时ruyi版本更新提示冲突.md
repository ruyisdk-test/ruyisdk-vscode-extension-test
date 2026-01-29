# 开启vscode时ruyi版本更新提示冲突

## 操作步骤

1. 正确安装多个版本的 ruyi，并且在 VSCode 中的 ruyi 包管理器可以自由切换版本
<img width="604" height="91" alt="ruyi multi-version normal switching" src="https://github.com/user-attachments/assets/8b70df38-af28-40d5-a515-a5a9c4c8dd78" />

2. 用旧版本打开 Visual Studio Code

## 预期结果
ruyi会弹出新版本ruyi的更新提示，询问是否更新。

## 测试结果
如果已经成功安装了最新版的 ruyi，那么在使用较旧版本的ruyi时打开vscode时，系统仍会提示是否需要更新 ruyi 包管理器的最新版本以及是否需要进行更新操作，如操作步骤可以正常切换版本，但类似于无法识别当前已安装了最新版本，使用旧版本就会提示更新最新版本。    
<img width="463" height="148" alt="图片" src="https://github.com/user-attachments/assets/85a440a8-0a69-4ca5-83b3-b14804ffd674" />
