# hma-scraper
Scrapes 16 pages of obfuscated proxy lists at proxylist.hidemyass.com

Why?
Excellent for when grey_harvest and tor dont provide enough IP address. This usually nets around 700 proxies.

storage format is full url, intended for instant curl -x usage
ex:
https://192.168.1.22:8080
socks5h://196.168.2.43:10000
http://192.168.3.23:8080


Requires: python 2.7+ or python3
modules used:
re, requests, print_function

Install:

$ git clone https://github.com/IDSninja/hma-scraper
$ cd hma-scraper
$ python hma-scraper.py > proxylist.txt

