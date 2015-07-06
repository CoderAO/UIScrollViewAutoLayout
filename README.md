这是一个简单的在storyboard中给UIScrollView子控件添加自动布局约束的示例.
给UIScrollView的子控件添加AutoLayout约束和其他普通的控件不同,因为scrollView需要根据子控件的尺寸和距离周围的边距来计算contentSize.

#####UIScrollView添加约束的正确方式如下:
- 首先,scrollView自身的约束(scrollView的位置和尺寸)可以像正常的UIView一样参照其父控件添加.
- 其次,scrollView内部子控件约束的添加需要遵循两个原则:
  - scrollView内部子控件的尺寸不能以scrollView的尺寸为参照
  - scrollView内部的子控件的约束必须完整

更进一步的介绍,请戳http://www.jianshu.com/p/258f4efd7a1d
如果有任何问题可以issue我~
