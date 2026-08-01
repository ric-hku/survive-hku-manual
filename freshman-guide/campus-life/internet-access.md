# 网络连接指南

## 一、校园 WiFi

学校的 WiFi 服务覆盖：

* 本部校园（含百周年校园）；
* 其他校园（沙宣道、玛丽医院、菲腊牙科医院等）；
* 学生宿舍；
* 其他港大办公场所（如坚尼地城中心、数码港等）。

一般在校园中，有以下三个 WiFi 可供连接：

### 1. HKU

是学校供教职工和学生使用的校内网络，可以使用 HKU Portal 账号访问。

配置方式：

* 用户名：HKU Portal UID
* 密码：HKU Portal PIN

{% hint style="info" %}
HKU Portal UID，指默认为 u3xxxxxx 的系统用户 ID。

修改 Email Alias 不改变 HKU Portal UID。
{% endhint %}

关于 Windows、MacOS、iOS、Android 及其他平台的配置方式，详见：[Procedures on Accessing "HKU" WiFi](https://its.hku.hk/kb/procedures-on-accessing-hku-wifi/)。

{% embed url="https://its.hku.hk/kb/procedures-on-accessing-hku-wifi/" %}

### 2. Wi-Fi.HK via HKU

供访客使用的 WiFi 服务，无需特殊注册、配置即可使用。

使用 Wi-Fi.HK via HKU 不能访问校内打印系统、理学院 OASS 等内部网络系统。

关于 Windows、MacOS、iOS、Android 及其他平台的配置方式，详见：[Procedures on Accessing Wi-Fi.HK via HKU](https://its.hku.hk/kb/accessing-wi-fi-hk-via-hku-service/)。

{% embed url="https://its.hku.hk/kb/accessing-wi-fi-hk-via-hku-service/" %}

### 3. eduroam

eduroam 即 [Education Roaming](http://www.eduroam.hk/)（教育漫游），是能够让教职工和学生在全球所有参与 eduroam 服务的院校和机构，使用本校的账号信息访问的 WiFi 服务。

使用 eduroam 不能访问校内打印系统、理学院 OASS 等内部网络系统。

配置完成后，可以直接在全球其他参与 eduroam 服务的院校和机构直接连接该 WiFi；同理，在其他院校和机构配置过 eduroam 的设备也可以直接连接港大的该 WiFi。

配置方式：

* 用户名：UID@hku.hk（UID，即 HKU Portal UID）
* 密码：HKU Portal PIN

关于 Windows 10、Mac、iOS、Android 及其他平台的配置方式，详见：[Procedures on Accessing eduroam WiFi Service](https://its.hku.hk/kb/accessing-eduroam-wifi-service/)。

{% embed url="https://its.hku.hk/kb/accessing-eduroam-wifi-service/" %}

## 二、HKUVPN

HKUVPN 是一个用于访问校园网络的渠道：当教职工、学生等处于校外时，可以使用 HKUVPN 安全地访问校园内部网络系统（如校内打印系统、理学院 OASS 等），就像身处校园一样。

如需使用 HKUVPN，必须配置多因素认证（MFA）。

### 1. 配置 MFA

多因素认证（MFA）要求用户访问 M365 账户时提供两种或以上验证方式。

MFA 能提升账户安全性，降低敏感信息被未授权人员获取的风险。

如果已配置 MFA，可跳过本节。

{% hint style="info" %}
自 2026 年 7 月 6 日起，所有学生从校外登录港大的各项网络服务（如 HKU Portal、HKU Moodle 等）时，均须使用 MFA。
{% endhint %}

可以选择以下方式接收令牌代码（Token Code）：

* 手机上的 Microsoft Authenticator 应用程序；
* 向手机号码发送短信（SMS）；
* 向手机号码通话（HKUVPN 不支持该种方法）。

建议在 MFA 中设置其他验证方式，以防万一主要方式无法使用。

关于如何配置 MFA，详见：[User Guide on Activating Multi-Factor Authentication (MFA)](https://its.hku.hk/kb/user-guide-on-activating-multi-factor-authentication-mfa/)。

{% embed url="https://its.hku.hk/kb/user-guide-on-activating-multi-factor-authentication-mfa/" %}

此外，建议检查自己在 ITS 处登记的备用电邮地址、电话号码是否可用：

* 在 HKU Portal 里选择 IT Support  &#x20;\> Register Contact Info with ITS（简体中文：资讯科技服务 > 注册联络资料）。

这里所登记的联系方式除了用于重置 HKU Portal PIN（密码），还可以用于**重置 MFA**。

### 2. 配置 HKUVPN

按照不同平台，查看有关配置方式、下载客户端的官方教程：

* [Windows](https://its.hku.hk/kb/setup-procedure-of-hkuvpn-with-multi-factor-authentication-mfa-for-windows/)
* [macOS](https://its.hku.hk/kb/setup-procedure-of-hkuvpn-with-multi-factor-authentication-mfa-for-macos/)
* [iOS](https://its.hku.hk/kb/setup-procedure-of-hkuvpn-with-multi-factor-authentication-mfa-for-ios/)
* [Android](https://its.hku.hk/kb/setup-procedure-of-hkuvpn-with-multi-factor-authentication-mfa-for-android/)
* [Linux](https://its.hku.hk/kb/setup-procedure-of-hkuvpn-with-multi-factor-authentication-mfa-for-linux/)

## 三、常见问题与解答

### Q1. 我无法连接到 HKU WiFi。为什么？

有可能是因为用户名输入错误。

请检查登录时输入的是默认格式为 u3xxxxxx 的系统用户 ID（HKU Portal UID）。

### Q2. 我在校内连接了网络，但无法访问打印服务（uPrint）。为什么？

有可能是因为设备连接的并非 HKU WiFi。

使用 Wi-Fi.HK via HKU、eduroam 不能访问打印系统等内部网络系统，必须是 HKU WiFi（或连接到 HKUVPN）。

### Q3. 连接 HKUVPN 时，客户端提示“登录失败”。怎么办？

请依次排查以下项目：

1. 确认用户名和密码正确。用户名须包含邮箱后缀（如 @connect.hku.hk）。
2. 确认一次性密码代码输入及时且准确。Microsoft Authenticator 的验证码每 30 秒刷新一次，若剩余时间较短，可等待刷新后再输入。
3. 确认学校 Microsoft 账号已添加 MFA 验证方式。若已添加，可删除当前 MFA 验证后，按官方指引重新配置。
4. 确认设备连接 HKUVPN 前，未连接其他代理工具。
5. 若以上方法均无效，可卸载 Cisco Secure Client，并按官方指引重新安装。

此外，也有可能是网络环境不稳定所致。可以尝试更换所连接的网络，多试几次。

### Q4. 我更换了我的手机 / 遇到了 MFA 相关的问题。怎么办？

ITS 提供了自行重置 MFA 的方式：[Reset HKU MFA](https://extranet.hku.hk/itpwdpol/servlet/resetMFA)。

可通过先前向 ITS 登记的备用电邮地址或电话号码来重置 MFA，无需联系技术支持人员。

如重置 MFA 无法解决问题，可尝试联系 ITS 的工作人员：

* 地址：Room 204, 2/F, K. K. Leung Building（现场 IT 支援）
* 电话：3917 0123（IT 支援、服务台）
* 电邮：[ithelp@hku.hk](mailto:ithelp@hku.hk)

***

想要加入 [RIC](../ric-intro/) 来一同为内地本科生维权益，谋福利吗？快快关注我们的微信公众号 **港大 RIC 锐克** 吧！我们将在九月发布招新信息哦～

本文作者：香港大学内地本科生权益保障组（RIC）；\
2025 修订作者：B27 冯雪菲 BASc(AppliedAI)；\
2026 修订作者：B27 陈斯涵 BSc(Bioinformatics)；B27 孙皋 BA。

本文基于原新生群文件《9.3 RIC教你科学上网》编写而成。

最后更新于 2026 年 8 月 1 日。

本文在知识共享 署名—非商业性使用—禁止演绎 4.0 协议（[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/deed.zh-hans)）下提供。
