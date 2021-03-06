# ZhihuDaily-Swift3.0
为了让我的另一个库WRNetWrapper使用起来更高效，特开此项目作为测试，代码从0开始

[知乎日报 API 分析](https://github.com/izzyleung/ZhihuDailyPurify/wiki/知乎日报-API-分析)

# 日志
#### **1.  2017.05.06**
- 完成启动页闪屏展示

**注意：**  
- 因为知乎素材并没有LaunchImage图片，所以我就用了自己App的启动图片。  
- 对喵神的 Kingfisher 修改了一下，解决了当placeholder为nil的时候，如果原图片框中已有图片，则会闪一下的问题  
修改后的代码  https://github.com/wangrui460/Kingfisher

---

#### **2.  2017.05.07**
- 重构网络部分代码

**注意：**  
- 以后所有网络请求都要放在 WRApiContainer 中。好处是所有网络请求一目了然、修改起来非常容易、类方法快速直接调用，基本不需要传什么参数！

--- 

#### **3.  2017.05.08**
- 完成版本更新检查

**注意：**  
- 因为不知道知乎日报的appid，所以点击前往后就跳到AppStore的首页


--- 

#### **4.  2017.05.09**
- 添加接口最新消息
- 启动页闪屏右上方添加跳过按钮，并添加点击事件

**注意：**  
- 用runtime写了一个UIView的分类，处理所有继承UIView的轻点事件  
- 把按钮添加在图片上，必须要设置图片isUserInteractionEnabled等于true，这样按钮才具有轻点事件

---


#### **5.  2017.05.10**
- 重构网络工具类，因为今天闪屏图片和版本检测的网络请求突然失效了
- 重构闪屏页上的跳过按钮事件
- 创建Story和News模型类，并且解析了一下最新消息返回结果

**注意：**  

-  取消直接在网络工具类中对成功返回结果转json操作，取而代之的是返回数组 response.result.value

---

#### **6.  2017.05.11**
- 导入第三方库MMDrawerController，实现基本抽屉效果
- 基本架构搭建完成

---

#### **7.  2017.05.15**
- 添加主页基本tableView
- 完成导航栏透明渐变效果
- 初步完成图片无线轮播效果

**注意：**

- 导航栏透明渐变效果使用了我的另一个开源框架  [WRNavigationBar_swift](https://github.com/wangrui460/WRNavigationBar_swift)
- 图片无限轮播功能使用了我的另一个开源框架[WRCycleScrollView](https://github.com/wangrui460/WRCycleScrollView)

---

#### **8.  2017.05.16**

- 完成主页的无线轮播效果，并且添加pageControl，解决滚动和拖拽过程中的一些bug

**注意：**

- 我就是给自己打广告，强烈推荐我的这两个框架   
- [https://github.com/wangrui460/WRNavigationBar](https://github.com/wangrui460/WRNavigationBar)   **求star，求包养**
- [https://github.com/wangrui460/WRCycleScrollView](https://github.com/wangrui460/WRCycleScrollView)**求star，求包养**

---

### 你觉得对你有所帮助的话，请献上宝贵的Star！！！ 不胜感激！！！
