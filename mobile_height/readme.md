## 移动手机网页高度问题
- flexible 10rem 问题 解决了宽度适配
- 单屏页面问题
    iphone6 667pt
    iphone6 Plus 736pt
    iphone5 568pt
    android 在iphone 5s -> iphone6 Plus -> 458宽
    一般不处理高度
    scroll-view  overflow:hidden|scroll
- height 同一设备在微信中，存在微信tabbar高度
    如做的网页是主要在微信中分享的，微信生态的
    应该使用微信开发者工具调试
- 解决不同手机的高度？
    其实不是手机高度的问题，单屏 要展示的内容不能太多，z-index+百分比缩放+定位去做
    微信生态 === h5生态
    基本的理念，height是有可为，有可不为，
    太多的内容，再放也放不下，如果安排得当，使用z-index+定位，在高度小的手机上，使用z-index去弥补高度不够的问题。
    单屏应用，不能太复杂
    等比例缩放？
    可使用vh rem media-query 等
- h5 单屏应用 不要急于下手 先构图
    有可能因为设计师缺少前端知识，介入进去，