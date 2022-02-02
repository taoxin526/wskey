
### 更新 · 摘要

#### Version 2022-02-02 新年快乐

---
**2022年2月2日 20:21:00**
- **修改检测青龙ID字段方法**
- **不再使用版本号作为判断依据**
- **移除更多废弃代码**

---
**2022年2月2日 15:51:42**
- **更新10.3.5接口**
- **新增`WSKEY_AUTO_DISABLE`变量 设置后不会自动禁用Cookie**
- **移除部分冗余代码**
- **感谢 `@Xeath` 的建议**

---
**2022年1月22日 11:19:41**
- **镜像地址 `https://hellodns.coding.net/public/sign/wskey/git/files`**
- **`ql repo https://e.coding.net/HelloDNS/sign/wskey.git "wskey"`**

---
**2022年1月14日 09:04:19**
- **修复2.10之前版本青龙失败问题**

---
**2022年1月13日 20:26:00**
- **修复2.11.0版本青龙检索失败重复添加问题**
- **此版本兼容旧版接口 无需担心**

---
**2022年1月13日 17:25:01** 
- **目前青龙版本2.11.0最好不要更新!!!**
- **还在修复Bug阶段 各种问题很多**

---
**2022年1月2日 14:41:20**
- **修正因青龙更换API导致的无法登录问题**

---
**2021年12月31日 12:43:03**
- **修复账号失效无法正常检测问题**

---
**2021年12月30日 13:25:23**
- **修复ConnectionResetError错误**
- **增加多节点测试功能**

---
**2021年11月23日 23:52:10**
- **~~新版青龙修改端口为5600了..~~**
- **脚本无需修改 如果出现报错的按照报错内容声明变量即可**

---
**2021年11月18日 21:05:20**
- **更新服务地址 务必更新!!!**
- **更新服务地址 务必更新!!!**
- **更新服务地址 务必更新!!!**

---
**2021年11月10日 14:16:45**
- **关闭自动禁用WSKEY**

---
**2021年11月3日 09:59:22**
- **新增面板登录失败推送**
- **修复出现错误码导致的脚本退出**

---
**2021年11月1日 18:53:45**
- **请使用甲骨文 等境外服务器的 检查自己的服务器DNS是否为 8.8.8.8**
- **国内服务器请使用 119.29.29.29 114.114.114.114**
- **排查一下午...客户机子上检查 居然是DNS不解析..出现异常退出的, 请先检查DNS服务器**

---
**2021年11月1日 16:50:25**
- **~~继续修复因为连接数过多导致的脚本异常~~**

---
**2021年11月1日 16:37:37**
- **~~尝试修复因为连接问题导致的脚本退出~~**

---
**2021年11月1日 12:34:20**
- **修复青龙推送失败导致脚本报错**

---
**2021年11月1日 06:07:22**
- **禁用时wskey&cookie同时禁用**
- **优化失效推送内容**
- **解决接口超时问题**

---
**2021年11月1日 03:18:01**
- **优化更新检查逻辑**
- **增加有效检查接口**
- **更新版本为 10.2.2**
- **修正接口错误问题**
- **引入随机签名算法**
- **引入随机 UA 算法**

---
**2021年10月28日 02:28:48**
- **使用修改sendNotify自动更新Cookie的朋友请务必 删除 `QL_WSCK` 变量**
- **否则会导致频繁更新Cookie导致Cookie有效期变得非常短暂** 
- **有Cookie自动禁用的程序可以开启 脚本转换后会自动启用转换成功的Cookie** 

---
**2021年10月10日 14:02:51**
- **修复因为长时间未登陆面板导致的Token失效 并修正Token获取**
- **感谢 @[haohaoget](https://github.com/haohaoget) 的 PR**

---
**2021年9月16日 19:31:24**
- **定时任务时间相同 同时请求过多 导致云端返回403**！！！
- **请大家务必修改定时任务的第一位时间！！！**
- **下个版本增加备选云端服务器和其他云参数地址**

---
**2021年9月16日**
- **继续修复定时任务错误的问题(莫名其妙的Bug)**
- **不使用可能引发执行错误的布尔判断**
- **云端更新UA**

----

**2021年9月15日**
- **继续修复定时任务错误**
- **移除LZMA GZIP等代码压缩 开放源码**
- **引入青龙面板推送功能 对脚本升级进行推送**

---
**2021年9月11日**
- **修复定时任务错误**

---
**2021年9月5日 (Ver: 905)**
-  **修改任务定时为`15 */16 * * *`**
- **增加 `QL_WSCK` 变量 填写变量后不检查Cookie有效性 直接进行转换** 

    > **最好修改定时任务为 16 小时 一次**

- **使用 LZMA 算法压缩脚本 更省空间**

- **修复一处升级逻辑判定错误**

---
**2021年9月4日 (Ver: 903)**
- **支持中文用户名的URL编码转换** 
- **封闭查询参数 改进对相似账号的搜索准确性**
- **HTTP请求加入异常捕捉, 并增加重试次数**
- **增加云端变量 从云端读取 UA 防止 UA 失效**
- **支持版本更新 有版本更新时 会提醒用户更新**
- **支持自定义端口 参数 `export QL_PORT="端口号" `**
- **优化逻辑部分 增加重试机制 对 API 接口增加备选方案**
- **支持实时输出日志 不需要等待执行完成才能看到结果**

---

### 使用方法

---

**原版地址** **`ql repo https://github.com/Zy143L/wskey.git "wskey"`**

**镜像地址 `ql repo https://e.coding.net/HelloDNS/sign/wskey.git "wskey"`**

**使用建议 修改定时计划 `15 */8 * * *`  ~~默认为8小时15分执行一次~~ 请按需修改**

---
### 变量声明

```shell
变量名: JD_WSCK 参数: pin=xxxx;wskey=xxxx;
# 注意分号 不要用中文分号!
变量名: QL_PORT 参数: 端口号(int) 
# 修改过面板端口的人才需要填写 默认 5700 
# 是本地的端口 不是 Docker 映射出去的端口! 如果你映射参数是 8888:5700 仍然填写5700
变量名: QL_WSCK 参数: 任意(str)
# 设置 QL_WSCK变量后 不检查有效性 直接更新 不使用请删除 而不是禁用
变量名: WSKEY_AUTO_DISABLE 参数: 任意(str)	
# 设置 WSKEY_AUTO_DISABLE变量后 不会自动禁用变量
```
---

### 程序特点

**1. 云端算法**

**2. 支持自定义内部端口的面板 例如 `5600  6666  3721` 对应变量 `export QL_PORT="端口号"`**

**3. 实时日志效果 无需全部执行完成返回**

**4. HTTP错误捕捉 最大限度防止出现因为容器没网 403错误 IP拉黑 等情况导致脚本错误**

**智能化**

   > **自动转换 JD_COOKIE 保证账号不过期**
   >
   > **自动添加 JD_COOKIE 保证账号不漏加**
   >
   > **自动更新 JD_COOKIE 保证账号不重复**

### 程序优点

----------------

​	**底层逻辑**打通**信息屏障**，创建脚本**新生态**。**顶层设计**聚焦用户感受

​	**抽离透传归因分析**作为**抓手**为产品**赋能**，**体验度量**作为**闭环**评判标准。

​	亮点是**载体**，优势是**链路**。思考整个**生命周期**，完善**逻辑**，考虑资源**整合**

-------------

### 干啥用的?

​	 用组合拳**赋能智慧**，打通**生态闭环**，帮助客户延长**有效时间**，强化用户**感知**，打破**边界**，打造**生态化薅豆**

---------------



