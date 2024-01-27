## 幻兽帕鲁私服部署

直接打开这个链接：

+ [https://hzh.sealos.run/?openapp=system-template%3FtemplateName%3Dpalworld](https://hzh.sealos.run/?openapp=system-template%3FtemplateName%3Dpalworld)

> 没错，你看到的就是 Sealos 的应用模板，这些模板可用于快速创建和部署网站和各种应用程序。你可以在模板市场中找到各种类型的模板，这些模板不仅包含了前端项目，还包含了后端和其他各类应用的部署，具体可参考 [Sealos 模板市场相关文档](https://sealos.run/docs/guides/templates/)。

接下来你只需要设置一下私服的管理员密码（ADMIN_PASSWORD）。

私服名称（SERVER_NAME）以及私服连接密码（SERVER_PASSWORD）是可选参数，如果你想给你的私服加上密码，就需要设置这两个参数，否则不用填。

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-15-35-uuZTOR.jpg)

然后点击右上角的「去 Sealos 部署」。

> 如果您是第一次使用 Sealos，则需要注册登录 Sealos 公有云账号，登录之后会立即跳转到模板的部署页面。

跳转进来之后，点击右上角的「部署应用」开始部署，部署完成后，直接点击应用的「详情」进入该应用的详情页面。

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-25-14-41-ciEYiI.png)

第一次启动私服会检查当前版本是不是最新版，如果不是最新版可能会在线更新一下。

等待应用变成 Running 状态，然后点击日志按钮查看日志，只要出现了下面的日志，便是启动成功了：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-25-12-25-4Ph7x4.jpg)

启动成功后，你可以关闭或者最小化「应用管理」App，然后回到「模板市场」的 palworld 应用界面，拉到最下面的「Others」，你会看到有一个类型叫「Service」的资源，它的描述部分有一个字段是这样写的：`8211:31039/UDP`，8211 后面的端口就是公网端口，比如这里的公网端口就是 31039。

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-23-22-41-vhHu8B.jpg)

那么你这个私服的地址就是 `hzh.sealos.run:31039`

大功告成，接下来开始登录游戏！

## 修改文件管理器密码

**这一步非常重要！！！为了防止别人能访问你的文件管理器，一定要修改密码！！！**

在「应用管理」界面进入 palworld 应用的详情页面，然后点击我用红框框出来的外网地址：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-09-6edDbv.png)

打开文件管理器后，输入用户名密码登录，默认的用户名是 `admin`，默认密码也是 `admin`。登录之后，先点击 "Settings":

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-12-LSucr2.jpg)

然后点击 "User management"，再点击 admin 最右边的铅笔按钮：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-26-LtKvG4.jpg)

在 "Password" 输入框中填入你的新密码，然后将 Language 的值改为「中文（简体）」：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-27-aWTOJm.jpg)

最后点击右下角的 save 即可。

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-27-bgXwUj.jpg)

## 登录游戏

首先需要[在 Steam 商店中购买幻兽帕鲁](https://store.steampowered.com/app/1623730/Palworld/?l=schinese)，然后登录 Steam 账号，在“库”中找到幻兽帕鲁，点击开始游戏，然后在游戏菜单中选择「加入多人游戏（专用服务器）」：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-23-22-57-Qp67If.png)

最后输入上面得到的私服地址，点击「联系」：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-23-23-26-CpxMYN.jpg)

然后就连接成功了！

如果你给私服设置了密码，那么你会遇到下面的报错：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-23-23-42-ql3yAi.jpg)

不要慌，我们上面不是设置了私服的密码嘛，所以需要输入密码才能连上，可是这里根本就没有让我输入密码的地方，仍然不要慌，听我指挥。先在「社群服务器」里找到一个带加密🔒的服务器，然后点击它：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-23-23-51-y1soiL.jpg)

这里输入你在部署私服时设置的密码，然后点击确定：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-23-23-53-TU7Haz.jpg)

接下来会问你要不要继续，**记住一定要选择「否」！**

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-23-23-54-JhhiKq.jpg)

最后再次点击私服地址右边的「联系」，就可以开始愉快地玩耍啦！

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-23-23-58-P11Jd0.jpg)

哦嚯，我进来了：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-23-23-21-AEyxOO.jpg)

看看国服的延迟多低👀

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-24-00-00-eiLXwZ.jpg)

## 私服高级玩法

如果你是个技术宅，略懂 Docker，可以研究一些更高级的参数设定，具体可参考模板所使用镜像的仓库地址：**https://github.com/thijsvanloef/palworld-server-docker**

Sealos 修改应用环境变量非常简单，只需要在应用详情页面点击右上角的「变更」按钮：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-24-00-57-RfScNI.jpg)

然后拉到下面的「高级配置」，点击「编辑环境变量」，就可以修改环境变量了。

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-24-00-57-xtXBw5.jpg)

举个例子，默认情况下应用每次启动时都会将私服更新到最新版本，但是国服到 Steam 的网络是不太通畅的，那么你就可以选择关闭自动更新。具体的做法是点击「编辑环境变量」之后，直接下面新增一行 `UPDATE_ON_BOOT=false`：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-25-12-23-8RwVvn.jpg)

然后点击「确认」，再点击右上角的「变更」，等待应用变成 Running 状态，然后点击日志按钮查看日志，只要出现了下面的日志，便是启动成功了：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-25-12-25-4Ph7x4.jpg)

具体可参考 [Sealos 官方文档关于环境变量的章节](https://sealos.run/docs/guides/applaunchpad/environment)。

## 省钱大法

最后我要上一个大杀器了，这个大杀器是个省钱大法。

由于 Sealos 是按量付费，所以我们可以想办法在自己不用的时候把这个私服给自动关掉，等需要用的时候再自动打开，岂不妙哉！

假设你每天上午 9 点到晚上 7 点在公司摸鱼打游戏，晚上回家拼命学习工作，那么你就可以搞个定时任务，**每天晚上 7 点自动将私服关停，每天早上 9 点再自动将私服开启**。

具体怎么做呢？

很简单，在 Sealos 桌面中打开「定时任务」：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-24-00-23-oa4lYb.jpg)

点击添加一个“**每天晚上 7 点自动将私服关停**”的定时任务，然后填入如下参数：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-24-00-25-0LYK2U.jpg)

1. 任务名称随便填，自己知道啥意思就行。

2. Cron 表达式设为每天下午 7 点执行。

3. 类型选择「执行命令」。

4. 镜像源选择 public。

5. 镜像名填入 `bitnami/kubectl`。

6. 运行命令填入 `bash -c`。

7. 命令参数填入 `kubectl scale sts palworld-fdbgshiv --replicas=0`。这里需要将 `palworld-fdbgshiv` 替换为你自己的 palworld 应用名，你的应用名可以到「应用管理」的 palworld 应用详情页面去看，我用红框框出来的部分就是 palworld 应用名：

   ![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-24-00-33-4liwjc.jpg)

然后点击「部署」即可。

接下来再创建一个“**每天早上 9 点再自动将私服开启**”的定时任务，参数如下：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-24-00-37-qFm9N1.jpg)

其他参数保持不变，只需要改变以下几个参数：

1. 任务名称，取一个自己知道意思的名字。
2. Cron 表达式设置为每天上午 9 点执行。
3. 命令参数和上面保持一致，只需要将 `--replias` 设置为 1，也就是 `kubectl scale sts palworld-fdbgshiv --replicas=1`。记住需要将 `palworld-fdbgshiv` 替换为你自己的 palworld 应用名。

最后点击「部署」大功告成。哎呀，这下省钱了，舒服！

如果你想在自己不玩的时候手动停止私服，只需要在应用详情页面点击右上角的「暂停」按钮即可：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-25-15-47-DaIwJ6.jpg)

**暂停之后 CPU 和内存均不收费，但是存储还是要收费的，因为存储一直占用在那边嘛~**

## 导出存档

在「应用管理」界面进入 palworld 应用的详情页面，然后点击我用红框框出来的外网地址：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-09-6edDbv.png)

双击我用红框框出来的 `Pal` 文件夹进入 `Pal` 文件夹：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-26-Ih0nOf.jpg)

然后单击我用红框框出来的 `Saved` 文件，再点击上方的下载图标：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-24-RHzR99.jpg)

点击我用红框框出来的 zip 即可将游戏存档压缩并下载到本地：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-25-Uuw8xg.jpg)

## 导入存档

将之前导出的存档解压成一个目录：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-29-SvOHiP.jpg)

在你的新私服「应用管理」界面进入 palworld 应用的详情页面，然后点击我用红框框出来的外网地址：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-09-6edDbv.png)

双击我用红框框出来的 `Pal` 文件夹进入 `Pal` 文件夹：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-26-Ih0nOf.jpg)

点击上传按钮：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-30-3ZrTIz.jpg)

选择上传文件夹：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-31-KON4x0.jpg)

然后选择本地的 Saved 目录进行上传，然后会出来一个弹窗，你只需要点击「替换」：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-33-1XMgM3.jpg)

上传完成后，回到「应用管理」的 palworld 应用详情页面，点击右上角的「重启」：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-16-35-8wt5Zp.jpg)

等待应用重启成功即可。

## FAQ

### 1. 如何调整私服的 CPU 内存？

在应用详情页面点击右上角的「变更」按钮：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-24-00-57-RfScNI.jpg)

然后可以随意调整 CPU 或者内存，最后点击右上角的「变更」即可。

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-25-14-45-JtJjsZ.jpg)

如果 8C16G 你还不满足，可以通过命令行来调整，不过比较复杂建议在群里联系 Sealos 官方人员帮你修改。

### 2. 如何估算成本？

在应用详情页面点击右上角的「变更」按钮：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-24-00-57-RfScNI.jpg)

在左边你会看到预估价格，**总价**就是每天的预估成本。

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-25-14-46-IxRoQi.jpg)

### 3. 如何删除密码？

参考上面的「私服高级玩法」章节，将 `COMMUNITY`、`SERVER_PASSWORD` 和 `SERVER_NAME` 这三个环境变量删除即可。

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-25-15-10-mri8k6.jpg)

### 4. 如何扩容存储

在应用详情页面点击右上角的「变更」按钮：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting-test@main/uPic/2024-01-24-00-57-RfScNI.jpg)

然后拉到最下面的「本地存储」，点击我用红框框出来的区域：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-25-15-32-RCvyqL.jpg)

将存储容量调整到你期望的数字（比如这里我调整到了 10G），最后点击「确认」，再点击右上角的「变更」即可。

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-25-15-31-2sOZo7.jpg)

### 5. 如何修改游戏参数？

在 Sealos 桌面点击「帕鲁配置器」：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-15-43-6hEA7t.jpg)

修改完参数后，点击「复制」：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-15-46-2FKOWt.jpg)

然后关闭或者最小化窗口，打开「应用管理」，进入 palworld 应用的详情页面，点击右上角的「变更」：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-15-47-xcncpG.jpg)

然后拉到下面的「配置文件」，点击我用红框框出来的区域：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-15-49-HcHet4.jpg)

然后将文件值中的所有内容都删掉，替换成刚刚在帕鲁配置器中复制的内容：

![](https://cdn.jsdelivr.us/gh/yangchuansheng/imghosting6@main/uPic/2024-01-27-15-51-ZyOGFZ.jpg)

## 私服交流群

最后，我们建了一个幻兽帕鲁私服交流qun，大家在部署私服的过程中如果遇到了什么问题，可以在qun里互相**深入**指导一下，QQ 群号：343680491