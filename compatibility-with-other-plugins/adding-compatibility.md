# 添加兼容性

添加兼容性到ItemsAdder物品是非常容易的！
**API**是**自由的**可通过maven包添加: [https://itemsadder.plugin.ga/developers/java-api](https://itemsadder.plugin.ga/developers/java-api)

## 如何获取项目

{% page-ref page="../developers/java-api/examples.md" %}

{% hint style="warning" %}
## 重要

请务必监听**ItemsAdderFirstLoadEvent**事件，ItemsAdder异步加载其物品和其他内容, 因此，在使用API之前必须等待此事件。
{% endhint %}

