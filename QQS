/*
KuWo music unlock vip
QX1.0.0:
^https?:\/\/api1\.talkmate\.com\/(talkshow\/homePage\/userInfo) url script-response-body https://raw.githubusercontent.com/295971920/QuantumultX/master/QQS.js
MITM = vip1.kuwo.cn
*/

var body = $response.body;
var url = $request.url;
var obj = JSON.parse(body);

const vip = '/talkshow/homePage/userInfo';

if (url.indexOf(vip) != -1) {
	obj.data["end_time"] = "18000000000";
	obj.data["member_type"] = "1";
	obj.data["money"] = "999";
	obj.data["month_num"] = "999";
	obj.data["start_time"] = "1588174515";
	body = JSON.stringify(obj);
}

$done({body});
