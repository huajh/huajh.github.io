---
layout:     post
title: 		"markdown test"
subtitle:   "markdown"
author:     "huajh7"
catalog:    true
header-img: "img/post-bg-universe.jpg"
tags:
  - markdown  
date: 2017-4-4
---


## example of markdown


###  homepage 
[huajh7.com](http://huajh7.com)


### quotes


> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.
> 
> machine
> >  This is nested blockquote.
> 
>  Back to the first level.
> return shell_exec("echo $input | $markdown_script");

### pargraphs 
* Red
+ Bule
	* machine
- good
1. Bird
2. parish

~~strik through~~

`import tempfile; print(tempfile.gettempdir())`

==hightlight==

-----------------------------------------
 


### 代码段和代码高亮

using `molokai.css`  by 
``rougify style molokai > css/syntax.css ``

Add the code in `syntax.css` to change the font and font-size

```css
.highlight {
  color: #F5F5F5;
  background-color: #272822;  /*#1b1d1e  f8f8f2  272822*/
  font-family: 'Consolas', serif;
  font-size: 15px;  
}
```


`ruby`
{% highlight ruby %}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}

<code class="hljs livecodeserver">{% highlight ruby %}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}</code>

`ruby`

```ruby
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
```

`matlab`

```matlab
A = cat( 3, [1 2 3; 9 8 7; 4 6 5], [0 3 2; 8 8 4; 5 3 5], ...
                 [6 4 7; 6 8 5; 5 4 3]);
% The EIG function is applied to each of the horizontal 'slices' of A.
for i = 1:3
    eig(squeeze(A(i,:,:)))
end
```

`python`

```python
class ReqStrSugRepr(type):

    def __init__(cls, name, bases, attrd):
        super(ReqStrSugRepr, cls).__init__(name, bases, attrd)

        if '__str__' not in attrd:
            raise TypeError("Class requires overriding of __str__()")

        if '__repr__' not in attrd:
            warn(
                'Class suggets overrding of __repr__()\n',
                stacklevel=3)
```


`c/c++`

```c
int main()
{
    int a = 10;
    print("int a = %d\n", a);
}
```


```java
import JavaBeans.People.Administor;

public class AcceptMember extends HttpServlet {

    /**
     * Constructor of the object.
     */
    public AcceptMember() {
        super();
    }

    /**
     * 
     * @throws ServletException if an error occurred
     * @throws IOException if an error occurred
     */
    public void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {

        response.setContentType("text/html");
        doPost(request, response);
    }
}


```


质能方程公式：$$E=mc^2$$

$$\min_{x,y} \sum_{i=1}^{N} (x_i+ 10 + y_i)^2 $$



### 脚注（footnote）

实现方式如下:

比如PHP[^1] Markdown Extra [^2] 是这样的。

[^1]: Markdown是一种纯文本标记语言

[^2]: 开源笔记平台，支持Markdown和笔记直接发为博文


### 引用方式：
I get 10 times more traffic from [Google][1] than from [Yahoo][2] or [MSN][3].  


### 下划线

---下划线---

### Images 

#### 内联方式：

![lenaNoise](/img/lenanoise.jpg "lenaNoise")


#### 引用方式：
![alt text][id] 

[id]: /img/mona-leber-final.jpg "mona-leber"


![]()



[1]: http://google.com/        "Google" 
[2]: http://search.yahoo.com/  "Yahoo Search" 
[3]: http://search.msn.com/    "MSN Search"


  


  


  


  


  


  


  


  


  


  


  




 







