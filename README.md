- [Useful Command](#useful-command)
  - [WSL与物理机通信,添加防火墙规则](#wsl与物理机通信添加防火墙规则)
  - [修改终端文件夹背景颜色](#修改终端文件夹背景颜色)
  - [git提交忽略文件](#git提交忽略文件)
  - [移动指定后缀到目录下](#移动指定后缀到目录下)
  - [javacp 打包class -> jar](#javacp-打包class---jar)
# Useful Command
## WSL与物理机通信,添加防火墙规则
`PS C:\WINDOWS\system32>  New-NetFirewallRule -DisplayName "WSL" -Direction Inbound  -InterfaceAlias "vEthernet (WSL)"  -Action Allow`
## 修改终端文件夹背景颜色
LS_COLORS="ow=01;36;40" && export LS_COLORS
## git提交忽略文件
`git config --global core.excludesfile ~/.gitignore`
## 移动指定后缀到目录下
`find . -name "*.log" -exec mv {} ../test \;`
`find ./ -name '*.log' | xargs cp -t test `
## javacp 打包class -> jar
`jar cvf xxx.jar \xx`