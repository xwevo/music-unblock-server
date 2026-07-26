本人纯小白0编程基础,我尽量说明白点.

generate-cert.sh和renew-cert.sh里可以改自签时间,有4个365我都改成3650了,server.crt自签后是10年,ca.crt还是5年,我是WIN10,你们啥系统签名时间太长了能不能用我也不知道,别问我.

env TYPE="RSA" ISSUENAME="Your Name" bash generate-cert.sh  执行这个代码可以自签,我是用GITHUB那个云端代码空间ai弄的,所以有问题别问我.

自签后下载ca.crt  server.crt  server.key

ca.crt跟着这个教程手动签名
https://github.com/UnblockNeteaseMusic/server/discussions/426

剩下的两个用环境变量里的这两个代码就可以接着用了,我也不知道你们用什么方法解锁的网易云,我是直接用别人写好的程序,所以怎么用也别问我.

SIGN_KEY=路径/server.key
SIGN_CERT=路径/server.crt

这是我用的程序,你们要用的话应该需要下载v0.28.0覆盖到里面.
https://github.com/FrzMtrsprt/QtUnblockNeteaseMusic
<img width="650" height="468" alt="image" src="https://github.com/user-attachments/assets/01299b2b-da59-43f8-bc71-6464d4d81a30" />
<img width="1323" height="940" alt="image" src="https://github.com/user-attachments/assets/c81784d0-ff95-421a-846b-357219583646" />
