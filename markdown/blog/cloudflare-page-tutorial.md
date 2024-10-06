---
title: 四步上线带域名的站点，cloudflare page 教程
date: 2024-10-04
---

### 1、注册Github并克隆项目

注册github，并登录

[https://github.com/signup](https://github.com/signup)

克隆模板

打开 [https://github.com/etrobot/AICodeSite](https://github.com/etrobot/AICodeSite)，按图创建新的项目

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image.png)

重新命个名称

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image1.png)

创建完成

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image2.png)

### 2、注册 Cloudflare Pages

[https://pages.cloudflare.com/](https://pages.cloudflare.com/)，注册账号

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image3.png)

连接github，选择刚才创建的项目

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image4.png)

选择框架

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image5.png)

开始构建

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image6.png)

构建成功

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image7.png)

访问地址：[https://cloudflare-page-nextjs-demo.pages.dev/](https://cloudflare-page-nextjs-demo.pages.dev/)，网页已经发布好了。

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image8.png)

### 3、注册域名

打开 [https://www.dynadot.com/](https://www.dynadot.com/)，搜索你想要的域名，例如：devfound.cfd（选了一个价格便宜的做示例）

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image9.png)

选中自己想要的，完成支付，在列表中可找到。

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image10.png)

点击进入域名DNS Settings

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image11.png)

选择 Name Servers，两个输入框中分别输入下面内容

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image12.png)

```bash
coleman.ns.cloudflare.com
miki.ns.cloudflare.com
```

### 4、绑定域名

进入 cloudflare页面，点击左边菜单 Workers & Pages，选择 Custom domain（想了解更多参考：[https://developers.cloudflare.com/pages/configuration/custom-domains/#add-a-custom-domain](https://developers.cloudflare.com/pages/configuration/custom-domains/#add-a-custom-domain)）

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image13.png)

输入刚才的domain

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image14.png)

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image15.png)

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image16.png)

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image17.png)

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image18.png)

按下图添加两条解析，content那栏填写：cloudflare-page-nextjs-demo.pages.dev，注意没有https之类。

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image19.png)

等一段时间激活（大概3-10分钟）

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image20.png)

再回到page项目的自定义域名页面，填写域名走一遍

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image21.png)

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image22.png)

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image23.png)

等待一段时间，大概1分钟激活成功。

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image24.png)

### 完成

访问：[https://devfound.cfd/](https://devfound.cfd/)，成功看到页面

![image.png](https://yu-r2-static.devfound.cfd/cloudflare-page-tutorial/image25.png)

项目地址：[https://github.com/callblueday/cloudflare-page-nextjs-demo](https://github.com/callblueday/cloudflare-page-nextjs-demo)