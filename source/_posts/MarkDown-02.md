---
title: MarkDown隐藏文字
date: 2023/03/08 12:30:00
categories: 
- Markdown
tags :
- 语法
cover: http://47.115.207.6/photo/Img/0-7.jpg
---

{% tabs %}
<!-- tab Inline -->

***inline 在文本里面添加按鈕隱藏內容，只限文字***

```
 content不能包含英文逗號，可用&sbquo;
```

content: 文本內容

display: 按鈕顯示的文字(可選)

bg: 按鈕的背景顏色(可選)

color: 按鈕文字的顏色(可選)

```
哪個英文字母最酷？ {% hideInline 因為西裝褲(C裝酷),查看答案,#FF7242,#fff %}

門裏站着一個人? {% hideInline 閃 %}
```




#### ***效果如下：***

{% hideInline content,display,bg,color %}

哪個英文字母最酷？ {% hideInline 因為西裝褲(C裝酷),查看答案,#FF7242,#fff %}

門裏站着一個人? {% hideInline 閃 %}
<!-- endtab -->

<!-- tab Block -->

block獨立的block隱藏內容，可以隱藏很多內容，包括圖片，代碼塊等等



```
( display 不能包含英文逗號，可用,&sbquo;)

{% hideBlock display,bg,color %}
content
{% endhideBlock %}
```

##### content: 文本內容

##### display: 按鈕顯示的文字(可選)

##### bg: 按鈕的背景顏色(可選)

##### color: 按鈕文字的顏色(可選)

#### 效果如下：

```
查看答案
{% hideBlock 查看答案 %}
傻子，怎麼可能有答案
{% endhideBlock %}
```

查看答案
{% hideBlock 查看答案 %}
傻子，怎麼可能有答案
{% endhideBlock %}

<!-- endtab -->

<!-- tab Toggle -->
如果你需要展示的內容太多，可以把它隱藏在收縮框裏，需要時再把它展開。

```
( display 不能包含英文逗號，可用&sbquo;)
{% hideToggle display,bg,color %}
content
{% endhideToggle %}
```

```
{% hideToggle Butterfly安裝方法 %}

他们都说  我好帅

为了追到我 想破脑袋

{% endhideToggle %}

```



#### 效果如下：

{% hideToggle Butterfly安裝方法 %}


他们都说  我好帅

为了追到我 想破脑袋

{% endhideToggle %}




<!-- endtab -->
{% endtabs %}