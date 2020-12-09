SendMessageModule
---------------

介绍
---------------
本模块可用于发送邮件和短信。

FROM: https://github.com/hongfeioo/messagemodule


调用方法举例
-----------------------------
```bash

#!/usr/bin/python
#coding=utf-8
import time

import messageMode


muti_phone = '135--------'
muti_mail = 'yihf@li.com'
arg_msg = 'baby,Be careful on the road'
begintime =  time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(time.time()))

messageMode.send_muti_sms(muti_phone,0,'hello baby',arg_msg)
messageMode.sendtxtmail('becare baby',0,arg_msg,muti_mail,begintime)
print 'ok'

```



参数介绍
--------------------
send_muti_sms 函数参数
> 1  手机号，当接受者为多人时用分号分割；</p>
> 2  默认为0，设置1则关闭所有短信报警</p>
> 3  短信标题,字符串格式.</p>
> 4  短信内容,字符串格式.</p>



sendtxtmail 函数参数
> 1  邮件标题</p>
> 2  默认为0，设置1则关闭所有邮件</p>
> 3  邮件正文内容</p>
> 4  邮件收件人，如果为多收件人则以分号分割</p>
> 5  发送时间</p>


邮箱,手机号,短信通道配置
----------------------------
```bash
vi messagemodule/messageMode.py 
```
>  muti_phone  接受报警短信的手机号，多手机号时用分号分割</p>
>  muti_mail   接受报警邮件的邮箱，多邮箱时用分号分割 </p>
>  pythonlog   运行日志的输出位置 </p>
>  sender      发件人的邮箱 </p>
>  smtpserver  发件服务器 </p>
>  username    发件邮箱用户名 </p>
>  password    发件邮箱密码 </p>
>  sms_string  短信通道字符串，这个需要你的公司有付费的短信通道,并配合修改第46行代码才可以使用。 </p>




开发环境
--------
Python 2.7.5 


作者介绍
----------
yihongfei  QQ:413999317    </p>
CCIE 38649


寄语
------
网工也能搞代码，为网络自动化运维尽绵薄之力! </p>
