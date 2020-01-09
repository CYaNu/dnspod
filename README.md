# 基于ArDNSPod修改的ddnspod脚本
主要用来在二级路由或者旁路由上更新DNSPod的域名DNS

具体操作：
  1 在dns.conf里面填入token和域名（第一位置为主域名如xxx.com,第二位置为二级域名如www）。
  2 复制文件夹到想要的位置，确认.sh文件权限。
  3 在crontab中添加定时任务，例如: */20 * * * * /usr/share/dnspod/ddnspod.sh 每20分钟更新一次。
  注：如路由器固件未集成完整版的curl，请在系统 软件包下安装curl。
  
更新版本：
  V1.0 发布   【测试环境ROS主路由+LEDE旁路由，运行在LEDE下】
