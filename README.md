# 路由器固件自动编译
[![OpenWrt](https://img.shields.io/badge/From-danxiaonuo-blue.svg?style=for-the-badge&logo=appveyor)](https://github.com/danxiaonuo/AutoBuild-Uola)
>固件来源：
[![UOLA](https://img.shields.io/badge/OpenWrt-UOLA-orange.svg?style=flat&logo=appveyor)](https://github.com/danxiaonuo/uola-os)

 ## 简介：
- 若 Fork 项目，请修改代码中自己的 TOKEN ( 项目 Settings/Secrets )

| TOKEN | 释义 |
| :--- | :--- |
| -- EMAIL  | Github用户邮箱 |
| -- SCKEY | Server酱SCKEY |
| -- UOLA_TOKEN | 个人 Settings/Developer settings/Personal access tokens新建获取 |

## 功能：
- 自动上传固件
- 自动发布固件
- 自动创建分支
- 自动上传到奶牛快传

## 变量：

| 变量名 | 释义 |
| :--- | :--- |
| -- REPO_URL="https://github.com/danxiaonuo/uola-os.git"  | 源码仓库地址 |
| -- REPO_BRANCH="main" | 源码分支 |
| -- TZ="Asia/Shanghai"  | 时区设置 |
| -- GITHUB_USER_NAME="danxiaonuo"  | Github 用户名 |
| -- GITHUB_USER_EMAIL="danxiaonuo@danxiaonuo.me"  | Github 邮箱 |
| -- GITHUB_RROJECT="github.com/danxiaonuo/AutoBuild-Uola.git"  | Github 编译仓库地址 |
| -- BRANCH="Uola_Hiwifi_Hc5962"  | 分支 |
| -- CONFIG_FILE=".config"  | 自定义.config文件名 |
| -- DIY_SH=""  | 定义脚本文件 |
| -- UPLOAD_BIN_DIR="false" | 上传 bin 目录 |
| -- UPLOAD_FIRMWARE="true" | 上传固件目录 |
| -- UPLOAD_BRANCH="true" | 上传分支 |
| -- CREATE_RELEASE="true" | 创建+上传发布 |
| -- BUILD_USER="danxiaonuo" | 编译者 |
| -- SEND_WECHAT_MSG="true" | 微信通知 |
| -- GITHUB_RELEASE="https://github.com/danxiaonuo/AutoBuild-Uola/releases"| 发行固件地址 |

##  默认配置
### 默认登录IP地址:10.8.1.1
###           用户:root       (路由 & SSH)
###           密码:admin      (路由 & SSH)

## 文件说明:

除提供已编译好的固件外，本项目还提供以下文件:

1. 完整性校验文件: sha256sums
2. Uola 编译配置: config.seed
3. 固件内已集成的软件包列表: manifest
