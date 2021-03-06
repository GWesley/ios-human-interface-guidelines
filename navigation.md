# 导航 (Navigation)

人们通常不会太注意一个 app 中的导航体验除非它没有满足他们的期望。你的工作就是实现一个可以支持应用结构和目的的导航并且不会过分引起用户的注意。

广义来说，有三种导航样式，每一个都能很好的满足特定 app 的结构：

* 分层。
* 扁平。
* 内容或体验驱动。

在一个分层式的 app 中，用户通过单一的选择来到达他们想去的位置。如果用户想去另一个地方，他们退回几步，或者从头开始，通过选择不同的选项。“设置”和“邮件”应用就是分层样式很好的例子。

<video src="images/navigation_hierarchy.m4v"></video>

在一个扁平结构的 app 中，用户可以直接从一个基本分类导航至另一个，因为所有的分类都列在主屏幕上。“音乐”和“App Store”是扁平结构的例子。

<video src="images/navigation_flat.m4v"></video>

在内容或体验驱动的结构中，导航是通过内容或用户体验进行的。例如，用户通过翻动页面或选择目录中的一页来看一本书；在游戏中，导航在很大程度上取决于用户体验。

<video src="images/navigation_contents.m4v"></video>

在某些情况下，一个 app 可以结合多种导航。例如，在扁平结构中，一个分类中的项目可能是分层结构的。

**用户应该永远都知道自己正处于 app 中的何处，也要知道如何前往下一个地点。**无论你使用何种导航模式，最重要的事情是用户前进的路径是有逻辑的、可预测的、容易实现的。

UIKit 定义了一些标准的 UI 元素，这使得实现分层结构和扁平结构的导航变得十分简单，此外，一些元素还可以帮助你实现内容驱动的导航，例如电子书或视频应用。像游戏或其他需要以用户体验驱动的应用通常依靠自定义的元素和行为。

**使用导航栏帮助用户轻松访问分层信息。**导航栏的标题可以显示用户当前在层次中的位置；返回按钮可以轻松回到上一级界面。想了解更多，请点击 [Navigation Bar](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW3)

**使用标签栏展示内容和功能的同级分类。**标签栏可以很好地展示扁平结构，用户可以在不同的分类之间随意切换。想了解更多，请点击 [Tab Bar](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW52)

**当 app 的每一页都有相同的项目或页面时，可以使用页面控制技术。**页面控制的优点是可以向用户展示可用的项目或页面，以及当前显示的内容。例如，“天气”应用使用页面控制来展示用户打开了多少特定地点的天气页面。想了解更多关于页面控制，请点击 [Page Control](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Controls.html#//apple_ref/doc/uid/TP40006556-CH15-SW6)

**通常情况下，每个页面都只有一条路径到达。**如果某个界面用户需要在多个地方进入，考虑使用临时视图，例如模态视图，动作菜单或警告框。想了解更多，请点击 [Modal View](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Alerts.html#//apple_ref/doc/uid/TP40006556-CH14-SW3), [Action Sheet](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Alerts.html#//apple_ref/doc/uid/TP40006556-CH14-SW36), [Alert](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Alerts.html#//apple_ref/doc/uid/TP40006556-CH14-SW2).

UIKit 也提供了以下的相关控制：

* [Segmented Control](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Controls.html#//apple_ref/doc/uid/TP40006556-CH15-SW27).一个分段控件可以让用户在一个屏幕下看到不同的分类或内容；并不需要导航至一个新的页面。
* [Toolbar](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW4).尽管工具栏看起来和导航栏或标签栏很相似，它也不能导航。相反，工具栏让用户可以控制当前页面的内容。
