OnionShare 是一个可以为我们提供，安全可靠的匿名文件分享的工具。通过它我们可以以匿名的方式，来共享我们任何大小的文件。它通过启动一个 Web 服务器，使其作为 Tor 洋葱服务进行访问，并且生成一个不可预测的 URL 访问，来提供文件的下载。它不需要在互联网上设置服务器，或使用第三方的文件共享服务。您只需要在自己的计算机上托管文件，并使用 Tor 洋葱服务，建立一个互联网的临时访问 URL 。其他用户只需使用 Tor 浏览器连接到该临时访问，便可下载到你的共享文件了。

特点：

 1.友好的用户图形拖放界面，并适用于 Windows，Mac OS X 和 Linux 系统。
 2.能够一次性共享多个文件和文件夹。
 3.支持多人同时下载文件。
 4.自动将临时访问 URL 复制到剪贴板。
 5.显示文件传输的进度。
 6.当文件完成传输后，OnionShare 会自动关闭，以减少被攻击面。
 7.支持多种本地化语言，并支持国际通用 unicode 编码文件名。
“如果你使用像 Dropbox 或 Mega 或 任何其它文件共享服务，你首先必须要建立在信任它们的基础上，才能使用它们。但不幸的是，它们往往会落到执法者手中，并成为有力的证据 。而 OnionShare 则允许您绕过所有第三方，并利用 Tor 网络让你在完全匿名的环境下，安全的将你的文件共享给其他用户。”——Micah Lee
当用户想要发送文件时，OnionShare 程序会在 Tor 网络上，创建受密码保护的临时站点 —— 所谓的 Tor 匿名服务 —— 在其计算机上运行。他们向收件人提供该站点的 URL 地址及连接密码。（这里最好使用那些通过 PGP 或 Off-The-Record 加密的即时通讯邮件。）收件人只需在 Tor 浏览器中，访问该临时 URL，就可下载到他人所共享的文件。

一旦其他用户成功下载完你的共享文件，你就可以取消该 web 服务，使链接永久失效。这样任何其他人，都将无法再访问该文件！

如何使用

在共享你的文件之前，你首先需要在后台，打开你的 Tor 浏览器 。这将会提供给你一个 Tor 服务，并提供给 OnionShare 以启动洋葱下的服务。

打开 OnionShare 并拖放你要共享的文件和文件夹，然后单击开始共享按钮 。它会回显你一个 .onion 的网址，如 http：//asxmi4q6i7pajg2b.onio/egg-cain 这样的，并将其复制到剪贴板 。这个 URL 用来下载你共享文件的私密网址。如果您希望多个用户能够下载该共享文件，那么请取消选中“自动关闭”复选框。

将此私密网址，发送给你想要发送文件给他的人。注意：如果你发送文件只是一般的普通文件，您可以使用正常的方式发送你的 URL，例如：发送电子邮件，发布到 Facebook 或 Twitter 上等。相反如果你发送的文件比较重要，那么你就必须要使用更加安全的方式来传送你的 URL 地址。

接收文件的人不需要 OnionShare。他们只需要在 Tor 浏览器，打开你发送给他们的 URL，便能够下载文件。

命令行下的使用

在 Linux 下，我们只需在 terminal 终端输入： onionshare 即可 。

在 Windows 下，只需将 C:\Program Files (x86)\OnionShare 添加到 PATH 环境变量下，之后在命令行下运行: onionshare.exe 即可 。

在 Mac OS X 下，我们首先在 terminal 下运行: ln -s /Applications/OnionShare.app/Contents/MacOS/onionshare /usr/local/bin 这条命令，然后在 terminal 下输入： onionshare 即可 。

当发件人想要对收件人保持匿名时，使用 Onionshare 无疑是最佳的选择。 如果举报人可以安全地向记者发送 Onionshare URL 和密码，那么他们就可能会使用它来泄露一些秘密信息，而不会被曝光身份。例如，维基解密 和 新闻组织 使用匿名泄漏软件 SecureDrop 来为他们自己提供 Tor 隐藏服务。Onionshare 可以给告密者更有效的保障，帮助他们像那些没有匿名提交系统的记者发送秘密信息。

OnionShare 保护了什么

第三方无权访问正在共享的文件。 文件直接托管在发件人的计算机上，不会上传到任何第三方服务器上 。相反，发件人的计算机则成为了文件共享服务器。这有别于传统的文件发送方式（例如：在电子邮件中或使用云托管服务）则需要信任该服务，才能访问到共享文件。

网络窃听者不能窥探到传输中的文件。 因为 Tor onion 服务和 Tor 浏览器之间的连接是端到端加密的。因此，当收件人进行文件的下载时，攻击者不可能截获到共享文件数据 。如果窃听者位于发送者端，接收者端，或者是恶意的 Tor 节点。那么，他们也只能探测到 Tor 的流量而已 。如果窃听者处在接收者的 Tor 客户端与发送者的 Tor  服务的交汇节点上，则通讯流量也将会被 Tor 服务密钥来进行加密传输。

发件人和收件人的匿名性由 Tor 提供保护。 OnionShare 和 Tor 浏览器 保护用户的匿名性。只要发件人使用 OnionShare URL 匿名地与接收者通信。那么，接收者和窃听者就不会知道发件人的真实身份。

即使攻击者枚举洋葱服务，共享文件仍然安全 。 目前，已经有针对 Tor 网络的攻击，可以枚举出洋葱服务。 但是即便有人发现了 OnionShare 洋葱服务的 .onion 地址，如果他们不知道 slug ，那么他们仍无法下载到共享文件。slug 是从 6800 个词的列表中，随机选出 2 个词生成的，这意味着它存在 6800 ^ 2，约 46 万种可能性 。而 OnionShare 只允许用户 20 次的错误机会，因此暴力破解的方式将会失效。除此之外 ，OnionShare 服务器还会使用常量时间字符串比较函数，来检查请求的 URI。因此，定时攻击也不能起到很好的攻击效果。

OnionShare 保护不了什么

OnionShare URL 的传送方式可能并不安全 。发件人通过安全的传输渠道将 OnionShare URL 发送给接收者 。如果他们采用不安全的发送渠道（例如：通过受攻击者监控的电子邮件），那么窃听者将知道，他们正在使用 OnionShare 来发送文件。此时，如果攻击者在合法收件人之前获取到 OnionShare URL，并迅速的使用 Tor 浏览器加载。那么，他们将可以下载你所共享的文件。因此如果是重要的文件共享，请务必使用例如：加密的电子邮件，聊天或语音中来传送 URL 。 

OnionShare URL 的传送方式可能并不安全 。 虽然 OnionShare 和 Tor 浏览器允许匿名发送文件，但是如果发件人也希望保持匿名性，那么就需要采取一些额外的措施，来发送 OnionShare URL 。例如，可以使用 Tor ，创建一个只能通过 Tor 访问的匿名电子邮件或聊天帐户，来共享你的 OnionShare URL 。

创建 OnionShare

首先从 github 上下载它的源码：

git clone https://github.com/micahflee/onionshare.git
cd onionshare
对基于.deb 的发行版（如 Debian，Ubuntu，Linux Mint）需要安装以下依赖包：

sudo apt-get install -y python3-flask python3-stem python3-pyqt5 python-nautilus
我们可以通过以下命令，来分别启动客户端或图形化界面的 OnionShare：

./install/scripts/onionshare
./install/scripts/onionshare-gui
以下是一个 a.deb 的安装脚本，利用该脚本我们就能更加方便的来安装 OnionShare 了：

sudo apt-get install -y build-essential fakeroot python3-all python3-stdeb dh-python python-nautilus
./install/build_deb.sh
sudo dpkg -i deb_dist/onionshare_*.deb
注意：OnionShare 是使用 stdeb 来生成 Debian 软件包的，而 python3-stdeb 在 Ubuntu 14.04（Trusty）中不可用。因此，您不能使用 build_install.sh 脚本，在 Ubuntu 14.04 以及更早版本 中，构建 .deb 文件 。

对基于 .rpm 的发行版（如 Red Hat，Fedora，CentOS）：

sudo sudo dnf install -y rpm-build python3-flask python3-stem python3-qt5 nautilus-python
./install/build_rpm.sh
sudo yum install -y dist/onionshare-*.rpm
这里您可能需要使用 yum 来代替 dnf 。

对于 ArchLinux：

可以通过 PKGBUILD 来安装 OnionShare：

下载地址：https://github.com/micahflee/onionshare


![Client Screenshot](/screenshots/client.png)
![Server Screenshot](/screenshots/server.png)

