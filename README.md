# 联通余量(v3)
[源仓库](https://github.com/xream/scripts/tree/main/surge/modules/10010v3)
> 本库仅供学习交流，如有问题请看源仓库

## 使用教程-青龙
> 脚本经由本人简单修改方便小白使用，详细教程和原脚本请看源仓库

### 第一步
青龙拉取脚本
```
ql raw https://raw.githubusercontent.com/liyw0205/Unicom-traffic-monitoring/main/10010.js
```

修改定时
> 以下定时为15分钟运行一次
```
*/15 * * * *
```
> 以下定时为上午7点到晚上11点每15分钟运行一次
```
*/15 7-23 * * *
```
> 以下定时为上午7点到晚上11点每15分钟运行一次
```
*/30 7-23 * * *
```
更多定时请百度

### 第二步
添加账号信息
脚本管理里找到脚本，在57行添加手机号,59添加服务密码,67行添加APPID
> APPID可以通过抓包及其他方法
<img src = "https://github.com/liyw0205/Connection-margin-v3-/blob/main/%E8%84%9A%E6%9C%AC/%E6%9D%A5%E6%BA%90/IMG_20221116_152154.jpg" >

### 多用户
把脚本复制并重命名即可，一个脚本一份账号信息
> 如10010_2.js 10010_3.js以此类推
缺点是会生成同一个10010-box.dat，导致某些信息错误
解决办法是新建文件夹，一个文件夹放一个脚本

### 推送
在配置文件config.sh里添加或者在脚本管理里sendNotify.js添加，脚本自动获取推送
> 推送怎么注册就不多说了

修改完成就可以开始跑了
<img src = "https://github.com/liyw0205/Connection-margin-v3-/blob/main/%E8%84%9A%E6%9C%AC/%E6%9D%A5%E6%BA%90/IMG_20221116_163812.jpg" >
<img src = "https://github.com/liyw0205/Connection-margin-v3-/blob/main/%E8%84%9A%E6%9C%AC/%E6%9D%A5%E6%BA%90/IMG_20221116_163757.jpg" >
