# ZipInstaller
破解 ZipInstaller.apk 方法

=================

应用名称：ZipInstaller.apk

应用包名：com.beerbong.zipinst

备注：应用提示 购买此应用及有广告

破解方法：

① 首先，反编译 ZipInstaller.apk，然后反编译 classes.dex。

② 找到 com/beerbong/zipinst/core/plugins/license/LicensePlugin.smali 文件并打开，定位到如下代码：

	# direct methods
	.method public constructor <init>(Lcom/beerbong/zipinst/core/Core;)V
    .registers 4

    .prologue
    const/4 v1, 0x0  //将 0x0 修改为 0x1

    .line 36
    const-string v0, "LicensePlugin"

    invoke-direct {p0, p1, v0}, Lcom/beerbong/zipinst/core/Plugin;-><init>(Lcom/beerbong/zipinst/core/Core;Ljava/lang/String;)V


【注意】 破解成功后，关于 → 购买 应用 菜单将显示为 关于 → 捐赠 。


按照上述标注修改然后保存。

最后编译，然后安装即可 。破解完毕！

=================

【特别声明】

👉 不保证上述破解方法永久有效！ 
如果此应用开发者重新修改代码，那上述破解方法就失效！这你必须要清楚明白！

👉 开发者敲字母编写程序代码也不容易，如果你条件(不管是经济还是网络条件)允许，还是请通过 Google Play商店 支付美元购买原版APK应用！以支持开发者的开发工作。

👉 我破解是因为我没有上述那个条件。穷逼无美元的破解者一个。 如果你愿意，请捐赠以支持我的破解工作。

👉 如果你还有问题？请 <a href=https://github.com/APK-Patched/ZipInstaller/issues>在此</a> 提交你的问题。
