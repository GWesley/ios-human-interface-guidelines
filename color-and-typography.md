#色彩和排版


>##色彩有助于增强通信


在iOS系统中，颜色用于表达互动性，传递活性，并提供视觉的连续性。内置的应用程序会使用那些看起来更有个性，纯净，干净的颜色，无论单独还是组合，还是在明或暗的背景下都看起来很不错。

![color_family_a_2x.png](images/color_family_a_2x.png)

**如果你想要创建多样自定义颜色，要确保他们可以很好地搭配在一起。**例如，如果你的应用程序主色调偏柔和，那么就应该建立一个协调的柔和色调的色板用于整个应用程序。

**注意在不同的环境下的颜色对比。**例如，如果导航栏的背景和按钮的标题没有足够的对比度，用户将很难看到按钮。根据经验，若想要判断应用程序的的颜色是否有足够的对比度，就是在不同的照明条件下用一个设备观察应用程序的视图，包括在晴朗的户外。

虽然在设备上查看你的应用程序可以帮助你找到你需要工作的地区，但是无法取代的一个更客观的方法获得的可靠结果。这种方法涉及确定前景和背景颜色亮度值之间的比率。为了得到这个比率，我们使用在线对比率计算器，或者你可以使用WCAG 2标准建立的公式自己计算。最理想的应用程序颜色对比度为4.5:1或更高。

**当你使用自定义的栏颜色时，要着重考虑半透明的栏和应用内容。**如果你需要创建一个色彩栏去匹配特的颜色，比如现有品牌的颜色，你可能不得不在得到你想要的结果前使用各种颜色进行试验。条栏的外观会受iOS系统提供的半透明和隐藏在栏后面的应用程序的内容显示影响。

>API注释
 使用着色（TintColor）的属性值给予栏按钮颜色，使用栏着色（BarTintColor）的属性值为栏本身赋色。欲了解更多关于栏属性的内容，可参见[UINavigationBar Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UINavigationBar_Class/index.html#//apple_ref/doc/uid/TP40006887)，[UITabBar Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UITabBar_Class/index.html#//apple_ref/doc/uid/TP40007521)，[UIToolbar Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIToolbar_Class/index.html#//apple_ref/doc/uid/TP40006927)和 [UISearchBar Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UISearchBar_Class/index.html#//apple_ref/doc/uid/TP40007529)。


**要注意颜色的盲区。**大多数色盲的人很难区分红色和绿色。需要测试你的应用程序，以确保没有用红色和绿色来作为区分两种状态或值之间的唯一途径的地方。一些图像编辑软件或工具，可以帮助你验证颜色的盲区。在一般情况下，使用多种方式来表示原色的交互性是一个好方法（了解更多iOS系统中关于表征交互性的内容，请看[互动元素Interactive Elements Invite Touch](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/InteractivityInput.html#//apple_ref/doc/uid/TP40006556-CH55-SW4))。

**选择一个基准的颜色来表征交互性和状态。**在内置的应用程序的基准色包括备忘录中的黄色还有日历中的红色等。如果你定义了一个表明互动性和状态的基准色，要确保你的应用程序中的其他颜色不会与其发生冲突。


**避免在交互式和非交互式的元素中使用相同的颜色。**颜色是一个UI元素显示其交互性的方式。如果交互式和非交互式的元素具有相同的颜色，用户会很难知道该点哪里。

**色彩可以传达信息，但不一定会以你期望的方式。**每个人眼中的颜色都是不同的，不同的文化差异赋予颜色的意义也是不同的。花时间去研究使用何种颜色可以被其他国家或者文化接受。你要尽可能地确保你应用程序中的颜色传达了恰当的信息。

**在大多数情况下，不要让颜色喧宾夺主。**除非色彩是应用的目的和本质所在，通常情况下色彩应该用来从细微细节之处提升用户体验。


##文本应该清晰易读

首先，文本必须清晰可见。如果用户不能读取应用程序的话，无论多么漂亮的排版也是没有意义的。当你的应用程序采用动态类型时，你可以实现：

* 能自动调整文字的粗细、间距大小和行高。
* 对语义不同的文本模块指定不同的文本样式，比如正文，脚注，或标题
* 文本可以根据用户在动态文字和可访问性设置中指定字体大小的变化作出适当的响应。（包括辅助文本大小）
 
>注意：如果你使用了自定义字体，你仍然可以通过系统提供的设置来调整大小。并且你的应用还应该在用户调整设置时做出合适的响应。

  对你而言，采用动态类型需要做的一些工作。要学习如何使用文本样式，并确保当用户更改文字大小的设置时，你的应用程序可以获取通知，可以参考[文本样式Text Styles](https://developer.apple.com/library/ios/documentation/StringsTextFonts/Conceptual/TextAndWebiPhoneOS/CustomTextProcessing/CustomTextProcessing.html#//apple_ref/doc/uid/TP40009542-CH4-SW65)。

**文本尺寸的响应式变化要优先考虑文本内容。**对用户来说，并不是所有的内容都是同样重要的。当用户选择一个更大的字体大小时，他们是想要自己关心的内容更容易阅读；并不是想屏幕上的每一个字都变大。

![mail_message_axlarge_2x.png](images/mail_message_axlarge_2x.png)

例如，当用户选择具备更大易用性的文本尺寸时，邮件通常会把主题和正文用较大的字体显示出来，而一些不那么重要的文本，比如日期、收件人等则采用较小的字体显示。

**当用户选择一个不同的文本大小时，要适当地调整布局。**例如，当用户选择一个较小的文本大小时，你可能要把正文从单栏式布局改成两栏式布局。你可以选择针对尺寸的子集来实现——如包含小，中和大尺寸——而不是对于每个可能的尺寸都进行布局的调整。

**确保一个自定义字体在不同尺寸下的所有类型都具备可读性。**实现这一效果的方法之一是模仿不同的文本尺寸下iOS系统呈现字体样式的一些方法。例如：

* 即使当用户选择特小号字号时，文本大小也不应小于11点（points）。相比之下，正文使用大尺寸的17点（points）的字号大小作为默认的字体大小设置。

* 一般情况下，字号与行距值在每一档的文本尺寸设置中差别为1点。唯一例外的是两种标题的样式，它们被应用在极小、小和中尺寸的设置中，使用了相同的字号、行距和字距。

* 在最小的三种字号中，字距值相对较大；在最大的三种字号中，字距相对比较紧凑。

* 标题与正文样式应使用相同的字体。为了和正文相区分，标题应使用更大的字号。

* 导航控制栏的文本使用相同的字号，而内容文本的样式则使用大尺寸的设置（值为17点）。

* 文字应使用常规或中等重量；不应使用轻的或加粗字体。

**在一般情况下，整个应用程序应使用一种单一的字体。**多种不同的字体混杂使用会使得应用程序显得草率而支离破碎。相反，使用一个字体和几种样式和尺寸。根据语义用法，使用[界面字体](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIFont_Class/index.html#//apple_ref/occ/cl/UIFont)的文本样式API来定义不同区域的文本样式，如正文或者标题。

推荐版

![font_choice_rec_2x.png](images/font_choice_rec_2x.png)

不推荐版

![font_choice_not-rec_2x.png](images/font_choice_not-rec_2x.png)
