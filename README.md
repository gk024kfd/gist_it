# gist_it

Gist_it can send to gist. 

  - anonymous mode
  - github login mode
  - public mode
  - secret mode

### Version
 2.7 was tested  
 
### Install
 pip install gist_it

### How to use
you can see help
```sh
gist_it -h
```
* anonymous mode and secret mode  
```sh
gist_it FILE_NAME
#or
cat FILE_NAME | gist_it
```
* anonymous mode and public mode  
```sh
gist_it FILE_NAME -p
#or
cat FILE_NAME | gist_it -p
```
* github login mode and secret mode  
```sh
gist_it FILE_NAME -a
#or
gist_it init # only first time
cat FILE_NAME | gist_it -a
```
* github login mode and public mode  
```sh
gist_it FILE_NAME -a -p
#or
gist_it init # only first time
cat FILE_NAME | gist_it -a -p
```
### Result
command result is 
```sh
https://gist.github.com/XXXXXXXXXXXXXXXXX
```

### Troble
```sh
#if this troble occurred

Traceback (most recent call last):
  File "/usr/local/bin/gist_it", line 5, in <module>
    from pkg_resources import load_entry_point
  File "/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/pkg_resources.py", line 2603, in <module>
    working_set.require(__requires__)
  File "/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/pkg_resources.py", line 666, in require
    needed = self.resolve(parse_requirements(requirements))
  File "/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/pkg_resources.py", line 565, in resolve
    raise DistributionNotFound(req)  # XXX put more info here
pkg_resources.DistributionNotFound: requests


#do this
sudo easy_install --upgrade pip
sudo pip install --upgrade setuptools
sudo pip install --upgrade distribute
sudo pip install --upgrade requests
```
