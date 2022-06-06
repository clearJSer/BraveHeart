# NVM 安装指南：

brew -v
安装homebrew：

```/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"```

使用homebrew 安装 nvm

brew install nvm

安装成功之后，还不能直接使用nvm命令，需要进行以下配置，将以下命令复制到终端执行：

```echo "source $(brew --prefix nvm)/nvm.sh" >> .bash_profile```

修改之后，需要重新定向来源，复制以下命令并执行：

```. ~/.bash_profile```

成功输入：
Nvm list

## 安装命令
nvm install node    安装最新版本
nvm install 8.16.0   安装指定版本

## 切换node版本
nvm use node      使用最新版本
nvm use 10.16.2  使用指定版本
例如：我在一个项目中使用的是node@10.16.2,新项目使用的是node@8.16.0,先要安装node@8.16.2，nvm install 8.16.2，然后，nvm use 8.16.2
