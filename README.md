## AntUI Reset  [原文] (https://antui.alipay.com/10.1.10/index.html#Reset%20or%20Normalize)

虽然文件名为reset，其实只是精简版的reset。

reset和normalize的区别可以看出，一个是控制倾向，一个是自然倾向。

精简版reset中，主要保留的是一些布局类reset（如margin:0），去掉了控制倾向比较强的部分。

同时，一些不常用的html5标签，也被去除。

## 特性

* **最低控制** 用户没有重置类样式时，也能保证基本显示
* **自由兼容** 使用者可以自由额外引入reset or normalize，而不用担心冲突
* **节约代码** 去掉一些不必要的代码，节约是良好的美德

````
*, *:before, *:after {
    -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
  }
  
  body, div, dl, dt, dd, ul, ol, li, h1, h2, h3,
  h4, h5, h6, form, fieldset, legend,
  input, textarea, p, blockquote, th, td {
    margin: 0;
    padding: 0;
  }
  
  table {
    border-collapse: collapse;
    border-spacing: 0;
  }
  
  fieldset, img {
    border: 0;
  }
  
  li {
    list-style: none;
  }
  
  caption, th {
    text-align: left;
  }
  
  q:before,
  q:after {
    content: "";
  }
  
  input:password {
    ime-mode: disabled;
  }
  
  /* A11Y：移除了 outline 样式，注意设置其他 :focus 样式，方便残障人士识别焦点 */
  *:focus {
    outline: none;
  }

````

