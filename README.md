# pay
银联支付

##银联下载地址
[zip](https://open.unionpay.com/ajweb/help/file/techFile?productId=3)

### 测试卡号
```java
    招商银行借记卡：6226090000000048
    手机号：18100000000
    密码：111101
    短信验证码：123456（先点获取验证码之后再输入）
    证件类型：01身份证
    证件号：510265790128303
    姓名：张三
```

### 调用支付控件
```
    // “00” – 银联正式环境
    // “01” – 银联测试环境，该环境中不发生真实交易
    String serverMode = "01";
    UPPayAssistEx.startPay (activity, null, null, tn, serverMode);
```

[![License](https://img.shields.io/badge/license-Apache%202.0-green.svg)](https://github.com/hugeterry/CoordinatorTabLayout/blob/master/LICENSE.txt)

![show](mipmap/ic_launcher.png)

![image](https://github.com/githubwing/DragPhotoView/raw/master/img/img.gif)

![这里写图片描述](http://img.blog.csdn.net/20151202143834990)

> **ExplosionField**，**爆炸效果发生的场地**，是一个View。当一个控件需要爆炸时，需要为控件生成一个ExplosionField，这个ExplosionField**覆盖整个屏幕**，于是我们才能看到完整的爆炸效果。
>
> **ExplosionAnimator**，爆炸动画，其实是一个**计时器**，继承自ValueAnimator。1024s内，完成爆炸动画，每次计时，就更新所有粒子的运动状态。**draw()方法**是它最重要的方法，也就是使所有粒子重绘自身，从而实现动画效果。
>
> **ParticleFactory**，是一个抽象类。用于**产生粒子数组**，不同的ParticleFactory可以产生不同类型的粒子数组。
>
> **Particle**，抽象的粒子类。代表粒子本身，必须拥有的属性包括，当前自己的**cx,cy坐标和颜色color**。必须实现两个方法，d**raw()方法选择怎么绘制自身**(圆形还是方形等),**caculate()计算当前时间，自己所处的位置**。
 <br><br>