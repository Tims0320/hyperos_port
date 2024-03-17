<div align="center">

# HyperOS 移植項目
### 基於 https://github.com/ljc-fight/miui_port

簡體中文&nbsp;&nbsp;|&nbsp;&nbsp;[English](/README_en-US.md)

</div>

## 簡介
- HyperOS 一鍵自動移植打包


## 目標機型及版本測試
- 測試機型小米10/Pro/Ultra MIUI 14最新版
- 測試版 小米12、小米13/Pro/Ultra、小米14/Pro HyperOS1.0 正式版及開發版 官方OTA包 & xiaomi.eu官改包
- 測試版本 小米平板5 Pro 12.4（DAGU）


## 正常工作

- 

## BUG

- 

## 說明



## 平板系統
移植平板HyperOS到手機，需要從其他正常手機HyperOS機型複製下面的軟體
Contacts MIUIAod MiuiHome MIUISecurityCenter Mms MIUIContentExtension MIUIPackageInstaller


## 如何使用
- 在WSL、ubuntu、deepin等Linux下
```shell
     sudo apt update
     sudo apt upgrade
     sudo apt install git -y
     # 克隆項目
     git clone https://github.com/toraidl/hyperos_port.git
     cd hyperos_port
     # 安裝依賴
     sudo ./setup.sh
     # 開始移植
     sudo ./port.sh <底包路徑> <移植包路徑>
```
- 在macOS下
```shell
     # 安裝brew
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

     # 克隆項目
     git clone https://github.com/toraidl/hyperos_port.git
     cd hyperos_port
     # 安裝依賴
     sudo ./setup.sh
     # 開始移植
     sudo ./port.sh <底包路徑> <移植包路徑>
```
- 在Termux上(未測試)
```shell
     pkg update
     pkg upgrade
     pkg install git tsu -y
     # 克隆項目
     git clone https://github.com/toraidl/hyperos_port.git
     cd hyperos_port/
     # 安裝依賴
     ./setup.sh
     # 進入root模式
     tsu
     ./port.sh <底包路徑> <移植包路徑>
```
- 上述程式碼中，底包路徑和移植包路徑可以替換為連結

## 感謝
> 本專案使用了以下開源專案的部分或全部內容，感謝這些專案的開發者（排名順序不分先後）。

- [「BypassSignCheck」by Weverses](https://github.com/Weverses/BypassSignCheck)
- [“contextpatch” by ColdWindScholar](https://github.com/ColdWindScholar/TIK)
- [「fspatch」by affggh](https://github.com/affggh/fspatch)
- [「gettype」by affggh](https://github.com/affggh/gettype)
- [「lpunpack」by unix3dgforce](https://github.com/unix3dgforce/lpunpack)
- [「miui_port」by ljc-fight](https://github.com/ljc-fight/miui_port)
- etc
