---
title: More on RESTful Communication
layout: page
permalink: /tutorials/s7
---


# Mod Rewrite with POST requests
To partition API to POST and GET APIs, you need to modify Apache config to include some conditions.
* Open your Apache config file, mine is located in `/etc/apache2/sites-available/000-default.conf`, and add the following with root permission
```xml
RewriteCond %{REQUEST_METHOD} ^POST$ [NC]
RewriteRule robot cgi/test.sh
``` 
The condition specifies how redirect the address based on request type. Check [Apache site](https://httpd.apache.org/docs/current/mod/mod_rewrite.html) for more details about `RewriteCond`. 
* Restart your Apache server
* To test POST request, you cannot use your browser easily because the browser operates mainly on GET part of HTTP (unless you use forms to submit data). Try `curl` command (`sudo apt install curl` if you don't have it on your system)
```bash
curl -X POST  '<address>/robot'
```
* Check if you receive correct HTML response ()





# Web communication in Python
It is quite easy to make HTTP requests in python using libraries like `requests`. Below is an example code.
* Lets make a simple GET request to your previously designed API. Create a file, named `req.py`  (or run interatively using ipython or Jupiter notebook )
* 
```python
import requests
url = '<ur server dns>/select/select/b'
x = requests.get(url)
print(x.text)
```

* If you run `print(x)` you will get HTTP response status code, which follows a standard protocol:
    1.  Informational responses (`100`–`199`)
    2.  <ins>Successful responses</ins> (`200`–`299`)
    3.  <ins>Redirection messages</ins> (`300`–`399`)
    4.  <ins>Client error responses</ins> (`400`–`499`)
    5.  <ins>Server error responses</ins> (`500`–`599`)
    Check [this link](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status#information_responses) for more details.
* You can replace `x = requests.get(url)` by `x = requests.post(url)` to run a POST request.  POST allows to attach additional content to requests. One famous attachements could be JSON file, a simple text-based data structure for key-value pairs (and more). So, you may modify the above code to attach an a content to your request.
```bash
myobj = {'somekey': 'somevalue'}
x = requests.post(url, json = myobj)
```