SendMessageModule
---------------

介绍
---------------
本模块可用于发送邮件和短信。


[单独运行的方法]
--------------------
```bash
python  messageMode.py    test123
```


[调用方法]
-----------------------------
```bash
import messageMode

messageMode.send_muti_sms(muti_phone,0,'hello baby log title',sms_msg)
messageMode.sendtxtmail('hello baby mail title',0,mail_msg,muti_mail,begintime)
```



[参数介绍]
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





开发环境
--------
Python 2.7.5 


作者介绍
----------
yihongfei  QQ:413999317   MAIL:yihf@liepin.com </p>
CCIE 38649


寄语
------
网工也能搞代码，为网络自动化运维尽绵薄之力! </p>
