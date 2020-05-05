# Markdown 语法

## 1、标题
使用 `#` 标记标题，从1级标题到6级标题，分别使用1到6个 `#` 。  

```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
``` 

_注意`#`号后的空格_

效果如下：  
> # 一级标题
> ## 二级标题
> ### 三级标题
> #### 四级标题
> ##### 五级标题
> ###### 六级标题

1级和2级标题也可以使用以下的标记方法：  
```markdown
一级标题
=======
二级标题
-------
```

效果如下：

> 一级标题
> =======
> 二级标题
> -------

## 2、段落

### 2.1 换行

markdown中需要换行时，可以在段末加两个以上的空格，或者加一个以上的空行：
```markdown
这是第一段  
这是第二段
```
或
```markdown
这是第一段

这是第二段
```

_加一个空行和加多个空行的效果相同。_

效果如下：
> 这是第一段
>
> 这是第二段

### 2.2 斜体和加粗

在文字两端加一个或多个`*`和`_`：
```markdown
_这是斜体_ 或 *这是斜体*
__这是加粗__ 或 **这是加粗**
___这是斜体加粗___ 或 ***这是斜体加粗***
```
_注意`_`或`*`号后没有空格_

效果如下：

> _这是斜体_ 或 *这是斜体*  
> __这是加粗__ 或 **这是加粗**  
> ___这是斜体加粗___ 或 ***这是斜体加粗***  

### 2.3 分隔线
三个或以上的`*`、`-`或`_`:
```markdown
***
---
___
```  

效果如下：
> ***
> ---
> ___

### 2.4 删除线

在文字两端加两个`~`：
```markdown
~~删除线~~
```

效果如下：
> ~~删除线~~

### 2.5 下划线
markdown本身不提供下划线，但可以使用html中的`<u>`标签来实现下划线。

```markdown
<u>这是下划线</u>
```

效果如下：

> <u>这是下划线</u>

### 2.6 注脚

可以用`[^ ]`来实现注脚：

```markdown
[^注脚]
[^注脚]: 注脚内容。
```

_但GitHub不支持这种语法。_

## 3、列表

### 3.1 无序列表

在列表项前加`*`、`+`或`-`：

```markdown
* 香蕉
+ 苹果
- 橘子
```

效果如下：
> * 香蕉
> + 苹果
> - 橘子

### 3.2 有序列表

数字加上`.`号：

```markdown
1. 第一项
2. 第二项
3. 第三项
```

效果如下：

> 1. 第一项
> 2. 第二项
> 3. 第三项

### 3.3 列表的嵌套

子列表项前加4个空格<kbd>Space</kbd>或者1个制表符<kbd>Tab</kbd>。

```markdown
* 这是父列表的第一项
    * 这是子列表的第一项
    * 这是子列表的第二项
* 这是父列表的第二项
```

效果如下：

> * 这是父列表的第一项
    * 这是子列表的第一项
    * 这是子列表的第二项
> * 这是父列表的第二项

## 区块

行首使用`>`：

```markdown
> 在我的后园，可以看见墙外有两株树，一株是枣树，还有一株也是枣树。  
> --鲁迅
```

效果如下：

> 在我的后园，可以看见墙外有两株树，一株是枣树，还有一株也是枣树。  
> --鲁迅

区块也可以像列表一样嵌套使用：

```markdown
>这是第一层
>
>>这是第二层
>>
>>>这是第三层  
>>  
>>这是第二层  
>  
>这是第一层
```

效果如下：

>这是第一层
>
>>这是第二层
>>
>>>这是第三层  
>>  
>>这是第二层  
>  
>这是第一层

## 代码

如果是单行的代码，可以用``` ` ```：

```markdown
`print('hello world')`
```

效果如下：

`print('hello world')`

如果是多行的代码，可以在每行的行首使用4个空格<kbd>Space</kbd>或者一个制表符<kbd>Tab</kbd>，也可以用三个`` ` ``包住代码块：

```markdown
    int main(){
        printf("hello world");
    }
```
或者
````markdown
```
int main(){
    printf("hello world");
}
```
````

效果如下：

    int main(){
        printf("hello world");
    }

当你使用三个`` ` ``时，你可以指定一种语言，来将：

````markdown
```javascript
$(document).ready(function(){
    alert("hello world");
})
```
````

效果如下：

```javascript
$(document).ready(function(){
    alert("hello world");
})
```

## 链接

```markdown
[GitHub](https://github.com)
```

或者

```markdown
<https://github.com>
```

效果如下：

> [GitHub](https://github.com)  

> <https://github.com>