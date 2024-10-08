# lhw-send-email

使用 pip install lhw-send-email 进行下载该库<br>
本库是作者第一个自主发布的三方库<br>

# 开发目的

为了完善自主开发的网站的验证码机制而做出的尝试

# 基本用法
1. 安装:
```
pip install lhw-send-email
```
2. 导入包
```
import lhw_send_email as lse

# 发送邮件功能(使用附件功能)
s = lse.SendEmail(fromEmailAddress=fromEmailAddress, password=password,
              destination=destination, subject=subject,
              content=content, isAtt=True, att_paths=att_paths)
```
3. 参数解释
```
SendEmail：
    fromEmailAddress: 格式 "Name <example@qq.com>"  <>中是邮件服务器(地址)-也可以是qq邮箱地址
    password: 邮箱授权码
    destination: 格式 "example@qq.com"  邮箱地址,不一定为qq邮箱
    content: 内容
    subject: 邮件标题
    api: 邮件服务器地址(默认为smtp.qq.com)
    isAtt: 是否携带附件(默认False,如果为True,则需要更改att_paths参数的内容)
    att_paths: 附件的路径
```
4. 具体用法
```
s.send()
```

# 关于bug反馈
1. 前往作者 [GitHub](https://github.com/fuyao-lhw/SendEmail 'SendEmail') / [Gitee](https://gitee.com/luo_hw/SendEmail 'SendEmail') 进行issues问题报告
2. QQ邮箱联系<br>
  1959415641@qq.com<br>
  1987239025@qq.com<br>
  fuyaoteam@gmail.com<br>

# 关于贡献以及PR提交
如果您发现任何问题或者有更好的优化策略及建议，可以在PullRequest处进行请求，
如若审核通过，我们将采纳您的方案，并记录您的贡献

