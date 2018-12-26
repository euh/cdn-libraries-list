# cdn-libraries-list

ajax.googleapis.com.txt doesn't contain all the JavaScript that ajax.googlesapis.com hosts (missing some old angular.js and yui).

code.jquery.com.txt contains all libraries hosted on code.jquery.com

You can use it to make your self hosted mirror and avoid potential tracking from google on ajax.googleapis.com or code.jquery.com and/or and speed up the display of websites.

More details :
- http://superkuh.com/ajaxgoogleapis.html
- https://github.com/rmm5t/googleapis-mirror

--
```
wget https://raw.githubusercontent.com/euh/cdn-libraries-list/master/ajax.googleapis.com.txt

wget https://raw.githubusercontent.com/euh/cdn-libraries-list/master/ajax.googleapis.com.txt

wget -x -nc -i ajax.googleapis.com.txt

wget -x -nc -i code.jquery.com.txt
```
