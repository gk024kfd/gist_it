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
