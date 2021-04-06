# 不兼容

_**它与X插件兼容吗？**_

我不能肯定地回答这个问题，因为我不知道世界上每个插件是如何编码的，但是这里有一些可能导致问题的插件列表:

* 所有使用 **自定义资源包** \(如果您对如何手动合并资源包有一点了解，则可以使它们兼容，请确保不要替换ItemsAdder文件，这样就完成了\)
* [CraftEnhance](https://www.spigotmc.org/resources/custom-recipes-and-crafting-craftenhance.65058/), 这个插件扰乱了ItemsAdder自定义配方逻辑，并造成了复制错误。所以请不要使用它
* [LootChest ](https://www.spigotmc.org/resources/lootchest.61564/)会引起一些 [问题](https://github.com/LoneDev6/ItemsAdder/issues/15#issuecomment-512990849)
* 目前插件**不兼容**生成不同面蘑菇块以创建自定义纹理的**插件**和**世界生成器**。将来我会添加兼容性。

