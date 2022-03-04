ff都市发展百叶帘20190825   5楼安装版本

2019-05-25 15:55:16  修改读取时间用 SD250 模块

2019-07-24 10:23:43 增加蓝牙名写入前清空

2019-08-01 14:10:22 增加开关切手动控制

2019-08-02 14:26:16 墙壁开关控制回自动控制 8H

2021-01-21
http post 请求返回503错误解析时没有数据体'{'错误

01-04 13:46:22I (73168) HTTP: ... set socket receiving timeout success

01-04 13:46:23r=192,recv=HTTP/1.1 503 Service Temporarily Unavailable

01-04 13:46:23Server: nginx/1.16.1

01-04 13:46:23Date: Mon, 04 Jan 2021 05:46:23 GMT

01-04 13:46:23Content-Type: text/html

01-04 13:46:23Content-Length: 91

01-04 13:46:23Connection: close

01-04 13:46:23ETag: "5ee899f7-5b"

if(strchr(recv_buf, '{')!=NULL)
{
    parse_objects_http_respond(strchr(recv_buf, '{'));
}

2021-02-03
http_send_mes(),DNS lookup failed err,增加return

2021-12-09
调整墙壁开关控制模式为高角联控模式

2022-03-03
本地计算高角联控
{"Command":"SetupProduct","Password":"CloudForce","ProductID":"69bcc8f08b4b407789f4868205ac819e","SeriesNumber":"DMO0005ILS1","Host":"mqtt.ubibot.cn","apn":"CMNET","user":"","pwd":""}

账号 dalianruban
密码 dalianurban12345

主要修改Motor_AutoCtl函数

MAX_AUTO_CTL_TIME 改为了 1 * 60

2022-03-04
增加串口debug指令
{"Command":"DebugOn","height":46,"angle":0}
{"Command":"DebugOff"}

增加捷昌遥控，兼容易佰龙和捷昌