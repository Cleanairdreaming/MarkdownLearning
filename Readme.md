MarkDown语法简介
=============================

下面是Markdwown的语法概述。  

## 一、标题  

### 1 Setext形式  
代码  
```markdown
H1
===
H2
---
=和-的数量无限制，只支持两级标题。
```  

### 2 atx形式  
代码  
```markdown  
# 一级标题
## 二级标题
###### 6级标题
```  


## 二、强调  
```markdown
斜体、黑体及两者结合
*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_
```  
`>>>`  
*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_

## 三、列表  
### 无序列表  
```
* Item 1
* Item 2
  * Item 2a
  * Item 2b
```  
`>>>`  
* Item 1
* Item 2
  * Item 2a
  * Item 2b

### 有序列表  
```
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
```
`>>>`  
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b

## 四、链接  
```
Markdown format: 
![Alt Text](url)
![logo](/images/logo.png)

Html format:
<img src="url" width="75" hegiht="75" align=center />
```  
`>>>`  
![logo](/images/logo.png)  
<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="75" hegiht="75" align=center />  

## 五、块引用
```
As Kanye West said:
> We're living the future so
> the present is our past.
```  
`>>>`  
As Kanye West said:  
> We're living the future so  
> the present is our past.  

## 六、行类代码
```
I think you should use an `<addr>` element here instead.
```
`>>>`  
I think you should use an `<addr>` element here instead.  

## 七、语法高亮
```python
# python with syntax highlighting
def test(a, b=1, *args):
    sum_ = a + b
    for arg in args:
        sum_ += arg
    return sum_, locals()
sum_, locals_ = test(1, 2, 3, 4)
>>>print(sum)
10
>>>print(locals)
{'arg': 4, 'sum_': 10, 'args': (3, 4), 'b': 2, 'a': 1}
```
