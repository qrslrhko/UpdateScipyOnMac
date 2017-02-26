### How to update new version of scipy on mac 

Refer to this problem on Stackfow http://stackoverflow.com/questions/26390895/why-isnt-pip-updating-my-numpy-and-scipy ,the below method shows how to fix it.

my old version is 0.16 and I want to update it to 0.17 

This is my old version of scipy:
```
>>> import scipy
>>> scipy.__version__
'0.16.1'
>>> scipy.__path__
['/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/scipy']
>>> 

```

For example, If I want to update my current version to [scipy 0.17.0](https://github.com/scipy/scipy/releases?after=v0.17.0rc2),I 
downloand the scipy-0.17.0rc1.tar.gz. 

The scipy is like in this directory :
 `/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/scipy`
(The 2.7 is my current Python version, you need to change it if we have fifferent version of Python)


After updating the version via pip, the new version will be stored in this directory  
`/Library/Python/2.7/site-packages`
(The 2.7 is my current Python version, you need to change it if we have fifferent version of Python)



## Here is the method to update the version of scipy which you want:

1. Step1: Delete the directory of scipy both in `/Library/Python/2.7/site-packages` and  `/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/scipy`

```
$ cd /Library/Python/2.7/site-packages
$ sudo rm -rf scipy

$ cd /System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/
$ sudo rm -rf scipy
```
2. Step2: Unzip the scipy-0.17.0rc1.tar.gz file and install it
```
$ tar -xvzf scipy-0.17.0rc1.tar.gz
$ cd scipy-0.17.0rc1
$ sudo python setup.py install
```

Let's check the version of scipy:

```
>>> import scipy
>>> scipy.__version__
'0.17.0rc1'
>>> scipy.__path__
['/Library/Python/2.7/site-packages/scipy']

```








