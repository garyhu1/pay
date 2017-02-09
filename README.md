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