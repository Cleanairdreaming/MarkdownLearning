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
# ```python
# <python script>
# ```

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

```
# python without syntax highlighting
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

## 八、任务列表
```markdown
- [x] @master, :smile:, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
  - [x] HTML
  - [x] CSS
  - [x] JavaScript
- [ ] this is an incomplete item
```  
`>>>`  
- [x] @master, :smile:, [links](#八、任务列表), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
  - [x] HTML
  - [x] CSS
  - [x] JavaScript
- [ ] this is an incomplete item

## 九、表格
```markdown
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

It seems like that, github doesn't support tables.
```
`>>>`  
| First Header | Second Header  |  
| ------------ | -------------  |  
| Content from cell 1 | Content from cell 2  |  
| Content in the first column | Content in the second column  |  

```html
<!-- use html Synopis instead -->
<table border="1">  
  <tr>  
    <th>Month</th>  
    <th>Savings</th>  
  </tr>  
  <tr>  
    <td>January</td>  
    <td>$100</td>  
  </tr>  
</table> 
```
`>>>`  
<table border="1">  
  <tr>  
    <th>Month</th>  
    <th>Savings</th>  
  </tr>  
  <tr>  
    <td>January</td>  
    <td>$100</td>  
  </tr>  
</table>  
