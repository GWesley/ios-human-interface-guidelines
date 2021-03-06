# 在应用中购买 (In-App Purchase)

应用内的购买服务使用户可以在你的应用、你设计的商店中购买数字产品。

![](images/in-app_purchase_2x.png)

例如，用户可能：

* 将一个应用从基础版升级到高级版
* 每月更新订阅的内容
* 购买虚拟商品，例如游戏中的等级或武器
* 购买并下载新书

你可以使用 StoreKit 技术在你的应用中嵌入一个商店并且支持应用内购买服务。当用户进行购买时，StoreKit 连接到应用商店进行安全支付，然后再告知你的应用来提供已购买的商品。

> **重要**
> 
> 应用内购买服务只提供支付功能，其他功能由你自己提供，例如向用户展示商品，解锁内置功能，从你自己的服务器上下载内容等等。当然，你所提供的所有商品都必须在应用商店注册过。
> 
想要了解添加购买功能的技术问题，请查看 [In-App Purchase Programming Guide](https://developer.apple.com/library/ios/documentation/NetworkingInternet/Conceptual/StoreKitGuide/Introduction.html#//apple_ref/doc/uid/TP40008267)。想要了解应用内购买的商业问题，请查看 [App Store Resource Center](http://developer.apple.com/appstore/)。当然，你还应该查看许可协议来确定你的应用出售哪些商品以及如何提供商品。

以下几点可以帮助你设计用户喜欢的购买体验。

**将商店体验无缝融合到你的应用中。**在展示商品和处理用户交易时，给用户提供一致性的体验。你一定不想让用户在访问你的商店时感觉进入了另一个不同的应用。

**使用简短简洁的标题和说明。**最好能让用户在扫过一组条目时快速发现感兴趣的内容。用户更容易理解简单直接的语言和标题。

**不要替换默认的确认提醒框。**当用户购买一个商品时，StoreKit 会提供一个确认提醒框（上方有展示）。这个提醒框可以帮助用户避免意外购买，所以不要修改它。
