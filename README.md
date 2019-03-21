# cdn-libraries-list

ajax.googleapis.com.txt doesn't contain all the JavaScript that ajax.googlesapis.com hosts (missing some old angular.js and yui).

code.jquery.com.txt contains all libraries hosted on code.jquery.com (missing some old jquery-ui css)

You can use it to make your self hosted mirror for speed up the display of websites or avoid potential tracking.

More details :
- http://superkuh.com/ajaxgoogleapis.html
- https://github.com/rmm5t/googleapis-mirror

Hints :
- You must create an HTTP and HTTPS server to answer requests and modify the hosts file on your system (or your DNS server if you have one).
- Because ajax.googleapis.com uses HSTS, for HTTPS requests you need to bypass your browser's protection. 
- For Firefox, use a hexadecimal editor to modify the file libxul.so or xul.dll (Windows) and alter what you find about ajax.googleapis.com
- You must repeat the operation after each update of Firefox
- I don't know the procedure for Chromium-based browsers.

--
```
wget https://raw.githubusercontent.com/euh/cdn-libraries-list/master/ajax.googleapis.com.txt

wget https://raw.githubusercontent.com/euh/cdn-libraries-list/master/code.jquery.com.txt

wget -x -nc -i ajax.googleapis.com.txt

wget -x -nc -i code.jquery.com.txt
```
