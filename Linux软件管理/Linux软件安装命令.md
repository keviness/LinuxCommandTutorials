## YUM安装软件
| 命令示例 | 描述 |
|:-------:|:---:|
yum install package_name | 下载并安装一个rpm包 
yum localinstall package_name.rpm | 将安装一个rpm包，使用你自己的软件仓库为你解决所有依赖关系 
yum update package_name.rpm | 更新当前系统中所有安装的rpm包 
yum update package_name | 更新一个rpm包 
yum remove package_name | 删除一个rpm包 
yum list | 列出当前系统中安装的所有包 
yum search package_name | 在rpm仓库中搜寻软件包 
yum clean packages | 清理rpm缓存删除下载的包 
yum clean headers  | 删除所有头文件 
yum clean all | 删除所有缓存的包和头文件 

## APT 软件工具 (Debian, Ubuntu 以及类似系统) 
| 命令示例 | 描述 |
|:-------:|:---:|
apt-get install package_name |安装/更新一个 deb 包 
apt-cdrom install package_name | 从光盘安装/更新一个 deb 包 
apt-get update |升级列表中的软件包 
apt-get upgrade |升级所有已安装的软件 
apt-get remove package_name |从系统删除一个deb包 
apt-get check |确认依赖的软件仓库正确 
apt-get clean |从下载的软件包中清理缓存 
apt-cache search searched-package |返回包含所要搜索字符串的软件包名称 

## DEB 包 (Debian, Ubuntu 以及类似系统) 
| 命令示例 | 描述 |
|:-------:|:---:|
dpkg -i package.deb |安装/更新一个 deb 包 
dpkg -r package_name |从系统删除一个 deb 包 
dpkg -l |显示系统中所有已经安装的 deb 包 
dpkg -l | grep httpd |显示所有名称中包含 "httpd" 字样的deb包 
dpkg -s package_name |获得已经安装在系统中一个特殊包的信息 
dpkg -L package_name |显示系统中已经安装的一个deb包所提供的文件列表 
dpkg --contents package.deb |显示尚未安装的一个包所提供的文件列表 
dpkg -S /bin/ping |确认所给的文件由哪个deb包提供 