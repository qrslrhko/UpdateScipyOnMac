## How to update new version of scipy on mac 

According to this problem on Stackfow http://stackoverflow.com/questions/26390895/why-isnt-pip-updating-my-numpy-and-scipy ,the below method is how to fix it.

Let's chenck my current version of Scipy on Mac terminal:

```
>>> import scipy
>>> scipy.__version__
'0.16.1'
>>> scipy.__path__
['/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/scipy']
>>> 

```
For example, I want to update my current version to [scipy 0.17.0](https://github.com/scipy/scipy/releases?after=v0.17.0rc2).
downloand the scipy-0.17.0rc1.tar.gz. 



### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```


### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/qrslrhko/chiaoyswebsite/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.


