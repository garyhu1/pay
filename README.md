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

### 对于新增的签名信息需注意以下几点
> **1.** 前台返回的支付结果中包含银联签名，要在商户后台对签名进行校验后才能展示结果。
>
> **2.** 前台签名使用的密钥和算法与后台结果中的签名一致。
>
> **3.** 如果商户APP在客户端内进行签名验证，要自行实现签名密钥更新的机制，否则更换密钥后会导致验签失败。**（不推荐）**
>
> **4.** 商户订单是否成功支付应该以商户后台收到全渠道返回的支付结果为准，此处支付控件返回的结果仅作为参考。
 <br><br>