版本更新如下
1：修复地图不加载或加载慢问题
2：优化一键安装
3：关机后一键启动功能
4：去除人物杂码
5：优化部分可修复偏移
一键搭建：
yum install git
git clone https://github.com/moonspell99c/PUBGradar.git
cd PUBGradar/
chmod u+x update.sh
./update.sh


重启后启动或打不开网页代码：
cd PUBGradar/
chmod u+x restart.sh
./restart.sh
慢步搭建：
wget --no-check-certificate -O shadowsocks-all.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-all.sh
chmod +x shadowsocks-all.sh
./shadowsocks-all.sh 2>&1 | tee shadowsocks-all.log
curl https://raw.githubusercontent.com/creationix/nvm/v0.13.1/install.sh | bash
source ~/.bash_profile
nvm install v9.8.0
nvm alias default v9.8.0
yum -y install gcc-c++
yum -y install flex
yum -y install bison
wget http://www.tcpdump.org/release/libpcap-1.8.1.tar.gz
tar -zxvf libpcap-1.8.1.tar.gz
cd libpcap-1.8.1
./configure
make
make install
yum install git
git clone https://github.com/moonspell99c/PUBGradar.git
cd PUBGradar/
npm i
npm i -g pino
npm install -g forever
forever start index.js sniff eth0 172.31.***.*** | pino

重启后启动或打不开网页代码：
cd PUBGradar/
chmod u+x restart.sh
./restart.sh
