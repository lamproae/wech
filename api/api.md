创建讨论组：
POST
https://wx.qq.com/cgi-bin/mmwebwx-bin/webwxcreatechatroom?r=“R”&pass_ticket=“pass_ticket”

POST格式：
{"MemberCount":MemberCount,"MemberList":[{"UserName":"UserName1"},{"UserName":"UserName2"}],"Topic":"","BaseRequest":{"Uin":Uin,"Sid":"Sid","Skey":"Skey","DeviceID":"DeviceID"}}


删除讨论成员

POST
https://wx.qq.com/cgi-bin/mmwebwx-bin/webwxupdatechatroom?fun=delmember&pass_ticket=“pass_ticket”
POST格式：
{"DelMemberList":"UserName1","ChatRoomName":"@@ChatRoomName","BaseRequest":{"Uin":Uin,"Sid":"Sid","Skey":"Skey","DeviceID":DeviceID"}}



增加讨论组成员：

POST
https://wx.qq.com/cgi-bin/mmwebwx-bin/webwxupdatechatroom?fun=addmember&pass_ticket=“pass_ticket”
POST格式：
{"AddMemberList":"UserName1","ChatRoomName":"@@ChatRoomName","BaseRequest":{"Uin":Uin,"Sid":"Sid","Skey":"Skey","DeviceID":"DeviceID"}}



#tips 
1. 不同的微信号登录域名是不一样的，有的微信号用wx.qq.com, 还有的账号用wx2.qq.com之类的域名。具体以初始化时返回的链接为准。
