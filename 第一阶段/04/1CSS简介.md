#CSS
- Cascading Style Sheets
- 层叠样式表
- 一个网页分三个部分:结构，表现，行为
  - 一个设计优良的网页把三个部分分离，降低代码耦合度
- 通过CSS可以为网页中的元素设置各种样式，优化页面  
- CSS编写位置
  - 内联样式表
    - `<p style="color:red; font-size:40px;">...</p>`
    - 直接将CSS编写到元素的style属性中 
    - 代码不易维护不推荐 
  - 内部样式表
    - 可以在head标签内部创建style标签，创建一个内部样式表 
    - 
    ```
    <style>
      p{//所有p元素都会改为相应样式
        color :red;
        font-size:40px;
      }
    </style>
    ```
    - 降低代码耦合利于维护
    - 内部样式表只能在当前页面中生效，无法在其他页面复用
    - 外部样式表 
    - 
    ```
    p{//例如文件名为style.css
      color :red;
        font-size:40px;
    }
    ```
    - 将样式编写到外部的CSS文件中,然后在head标签内通过link标签引入
    - `<link rel="stylesheet" href="style.css">`
    - 将结构和表现完全分离，易于维护，代码可以在不同页面复用，且外部文件可以利用浏览器缓存机制，加快访问速度