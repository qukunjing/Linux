# ubuntu_优化
## 系统优化
### 卸载libreOffice
`sudo apt-get remove libreoffice-common`
### 删除Amazon的链接
`$sudo apt-get remove unity-webapps-common` 
### 删除不常用的软件
```
sudo apt-get remove thunderbird totem rhythmbox empathy brasero simple-scan gnome-mahjongg aisleriot 
sudo apt-get remove gnome-mines cheese transmission-common gnome-orca webbrowser-app gnome-sudoku  landscape-client-ui-install  
sudo apt-get remove onboard deja-dup 
```
## 换源
### 阿里云
```
deb http://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ focal-proposed main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ focal-proposed main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse
```

## 系统时间
```
sudo apt-get install ntpdate
sudo ntpdata time.windows.com
sudo hwclock --localtime --systohc
```
## 软件安装
### 安装坚果云
```
https://www.jianguoyun.com/s/downloads
apt-get -f install 
dpkg -i 安装包
```
### 安装vim
`sudo apt-get install vim`
### 截图shutter
```
sudo add-apt-repository ppa:linuxuprising/shutter
sudo apt-get update
sudo apt install shutter
```
### 安装chrome
`sudo dpkg -i google-chrome-stable_current_amd64.deb`
### 安装WPS
```
https://linux.wps.cn/
sudo dpkg -i wps-office_10.1.0.5672~a21_amd64.deb
#if error
sudo apt-get install -f
```
### 解压缩rar
`sudo apt-get install rar`

### 网易云音乐
```
https://music.163.com/#/download 
sudo dpkg -i 安装包
```
### 安装pip3
`sudo apt-get install python3-pip`
### 安装GnomeTweak
```
sudo apt install gnome-tweak-tool
sudo apt-get install gnome-shell-extensions
```
### 安装VS Code
```
https://code.visualstudio.com/
sudo dpkg -i *vscode*.deb
```
### QQ&&WeChat
```
cd ~
mkdir deepinwine
cd deepinwine
touch install.sh
wget http://mirrors.hust.edu.cn/deepin/pool/non-free/d/deepin-wine/deepin-wine_2.18-22~rc0_all.deb
wget http://mirrors.hust.edu.cn/deepin/pool/non-free/d/deepin-wine/deepin-wine32_2.18-22~rc0_i386.deb
wget http://mirrors.hust.edu.cn/deepin/pool/non-free/d/deepin-wine/deepin-wine32-preloader_2.18-22~rc0_i386.deb
wget http://mirrors.hust.edu.cn/deepin/pool/non-free/d/deepin-wine-helper/deepin-wine-helper_1.2deepin8_i386.deb
wget http://mirrors.hust.edu.cn/deepin/pool/non-free/d/deepin-wine-plugin/deepin-wine-plugin_1.0deepin2_amd64.deb
wget http://mirrors.hust.edu.cn/deepin/pool/non-free/d/deepin-wine-plugin-virtual/deepin-wine-plugin-virtual_1.0deepin3_all.deb
wget http://mirrors.hust.edu.cn/deepin/pool/non-free/d/deepin-wine-uninstaller/deepin-wine-uninstaller_0.1deepin2_i386.deb
wget http://mirrors.hust.edu.cn/deepin/pool/non-free/u/udis86/udis86_1.72-2_i386.deb
wget http://mirrors.hust.edu.cn/deepin/pool/non-free/d/deepin-wine/deepin-fonts-wine_2.18-22~rc0_all.deb
wget http://mirrors.hust.edu.cn/deepin/pool/non-free/d/deepin-wine/deepin-libwine_2.18-22~rc0_i386.deb
wget http://mirrors.hust.edu.cn/deepin/pool/main/libj/libjpeg-turbo/libjpeg62-turbo_1.5.1-2_amd64.deb
wget http://mirrors.hust.edu.cn/deepin/pool/main/libj/libjpeg-turbo/libjpeg62-turbo_1.5.1-2_i386.deb

echo '准备添加32位支持'
sudo dpkg --add-architecture i386
echo '添加成功，准备刷新apt缓存信息...'
sudo apt update
echo '即将开始安装...'
sudo dpkg -i *.deb
echo '安装完成，正在自动安装依赖...'
sudo apt install -fy
sudo ./install.sh 
```
### VLC视频播放器
`sudo apt install vlc`
### steam
`sudo apt install steam`
### edge浏览器
`https://www.microsoftedgeinsider.com/zh-cn/download/`
### sogou拼音输入法
`https://www.jb51.net/article/186808.htm`
### 安装GIMP
`sudo apt install gimp`
### 邮件软件
```
https://getmailspring.com/download
sudo dpkg -i *.deb
```

### 下载软件uget
```
https://ugetdm.com/downloads/ubuntu/
sudo dpkg -i uget*.deb
sudo apt install aria2
###进入软件>编辑>设置>插件>改成aria2
###进入uget主页>右键左下角新建>属性>默认一般设置>修改下载位置>讲线程改成16
```
### ssr
```
sudo apt install libcanberra-gtk-module libcanberra-gtk3-module gconf2 gconf-service libappindicator1
sudo apt-get install libssl-dev sudo apt-get install libsodium-dev
sudo apt install python
sudo dpkg -i *.deb
electron-ssr
```
### Typoa
``` 
wget -qO - https://typora.io/linux/public-key.asc | sudo apt-key add -
sudo add-apt-repository 'deb https://typora.io/linux ./'
sudo apt-get update
sudo apt-get install typora
```
### 大部分软件
`https://blog.csdn.net/weixin_45225720/article/details/114403274?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522161823630616780274188526%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=161823630616780274188526&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_v2~rank_v29-12-114403274.first_rank_v2_pc_rank_v29&utm_term=ubuntu20.04%E5%AE%89%E8%A3%85%E8%BD%AF%E4%BB%B6`
## 常用命令
### 安装&卸载
`apt-get install softname apt-get remove softname`
### 软件卸载并清除配置
`apt-get remove -purge softname`
### 安装DEB软件包
```
sudo dpkg -i softname.deb
sudo dpkg -r xxx.deb
```
### 连同配置文件一起删除
`sudo dpkg -r --purge xxx.deb`
### 已安装软件包信息
`sudo dpkg -l`
### 解压.tar.gz文件
`tar -xzvf filename`
