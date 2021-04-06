# ⚙️首次安装

## 视频教程

{% embed url="https://youtu.be/GKGnlF4zZVg" %}

{% hint style="info" %}
**你应该在本地测试服务器上**进行第一次配置以**避免错误**和多次重启.. 玩家不喜欢服务器停机 ;\)   
你可以在完成所有配置后将文件上传到真实的服务器。
{% endhint %}

{% hint style="danger" %}
如果您已经拥有ItemsAdder旧1.0版本，请重命名**Plugins/ItemsAdder**文件夹为**ItemsAdder\_backup**
{% endhint %}

## 步骤 1 - 安装插件和API

* 安装 [**ProtocolLib**](https://www.spigotmc.org/resources/protocollib.1997/)
* 安装 [**LoneLibs**](https://www.spigotmc.org/resources/lonelibs.75974/)\*\*\*\*
* 安装 [**LightAPI**](https://www.spigotmc.org/resources/lightapi-fork.48247/)
* 将**ItemsAdder.jar**文件放入Plugins文件夹
* 启动服务器
* 让ItemsAdder完成加载**一切**
* 停止服务器

## 步骤 2 - 资源包首次安装

* 当插件完全加载后加入服务器并执行命令`/iazip`
* 打开Plugins\ItemsAdder\config.yml
* 如果要在服务器上直接托管资源包，请遵循本教程

{% page-ref page="plugin-usage/resourcepack-hosting/resourcepack-self-hosting.md" %}

* 如果您想在DropBox上托管资源包，你可以遵循本教程

{% page-ref page="plugin-usage/resourcepack-hosting/resourcepack-on-dropbox.md" %}

{% hint style="warning" %}
**每次**你想让插件更新`pack.zip`文件**记得**使用命令`/iazip`
{% endhint %}

## 可选步骤 - 删除默认物品

{% hint style="info" %}
如果你不关心我默认提供的物品，你只想添加自己的物品、方块和其它东西，这很简单！

{% page-ref page="faq/removing-default-stuff.md" %}
{% endhint %}



