DEPRECATED. They changed their site

# hma-scraper
This is a single python script that scrapes a specified number pages of obfuscated proxy lists at proxylist.hidemyass.com

hma obfuscated the html source with a lot of display:none elements. Never fear, regex is here.

###Why?
Excellent for when grey_harvest and tor dont provide enough IP addresses. 107 pages (current number of listed pages) is currently giving 5314 proxies.

Storage format is full url, intended for instant curl -x usage

ex:
```
https://192.168.1.22:8080
socks5h://196.168.2.43:10000
http://192.168.3.23:8080
```

###Requires:
python 2.7+ or python3

###Modules used:

re, requests, print_function, sys

###Install/Usage:
```
$ git clone https://github.com/IDSninja/hma-scraper
$ cd hma-scraper
$ python hma-scraper.py <number of pages to scrape> > proxylist.txt
$ python hma-scraper.py 107 > proxylist.txt
```

####See also:
Another good proxy harvester is grey_harvest:


https://pypi.python.org/pypi/grey_harvest/0.1.3.5
