# 初始化安装

在云服务器上部署 Joomla 预装包之后，请参考下面的步骤快速入门。

## 准备

1. 在云控制台获取您的 **服务器公网IP地址** 
2. 在云控制台安全组中，检查 **Inbound（入）规则** 下的 **TCP:80** 端口是否开启
3. 若想用域名访问 Joomla，请先到 **域名控制台** 完成一个域名解析

## Joomla 安装向导

1. 使用本地电脑的 Chrome 或 Firefox 浏览器访问网址：*http://域名* 或 *http://Internet IP*, 就进入引导首页

2. 选择一门语言，并设置站点名称
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/joomla/joomla-wizard1-websoft9.png)

3. 填写用户，账号，邮件等信息，然后进入下一步
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/joomla/joomla-wizard2-websoft9.png)

4. 填写您的数据库参数（[不知道账号密码？](/zh/stack-accounts.md#mysql)），然后进入下一步
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/joomla/joomla-wizard3-websoft9.png)

5. 安装成功，建议此时点击【特别推荐：安装语言】以安装更多语言以支持未来的多语言网
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/joomla/joomla-wizard4-websoft9.png)

6. 开始安装更多语言（可选），其中【Chinese Simplified (zh-CN)】是必选语言
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/joomla/joomla-wizard5-websoft9.png)

7. 根据提示，设置是否开启网站的多语言功能，并设置默认前后台语言
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/joomla/joomla-wizard6-websoft9.png)

8. Joomla后台地址：http://域名/administrator，成功登陆后您可以开始使用Joomla
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/joomla/joomla-wizard7-websoft9.png)
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/joomla/joomla-wizard8-websoft9.png)

> 需要了解更多 Joomla 的使用，请参考官方文档：[Joomla Docs](https://docs.joomla.org/Main_Page/zh-cn)

## 常见问题

#### 浏览器打开IP地址，无法访问 Joomla（白屏没有结果）？

您的服务器对应的安全组80端口没有开启（入规则），导致浏览器无法访问到服务器的任何内容

#### 本部署包采用的哪个数据库来存储 Joomla 数据？

是MySQL

#### 是否可以采用云厂商提供的 RDS 来存储 Joomla 数据？

可以

#### 当前 Joomla 不是最新版本怎么办？

完成 Joomla 初始化安装后，登录后台可以一键在线更新至最新版本