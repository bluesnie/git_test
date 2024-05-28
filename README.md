## 前言

- package.json 生成： `npm init`

- `gitbook install` 安装插件
    - 报错，需要按照 10.22.0 版本的node，使用 
    - [windowns nvm](https://www.cnblogs.com/zhangkq/p/14798270.html) 管理版本
    - [linux nvm](https://www.cnblogs.com/zhangkq/p/14798270.html) 管理版本
- 目录自己编写(自动生成插件生成的不好)
- `gitbook serve` 启服务~~，~~~~并且会生成目录~~
    - ~~需要执行 2 次，第一次生成目录，第二次才是~~生成内容页
- `npm run build` 生成电子书（修改了文档，记得及时执行此目录更新）
- docs 是网页电子书目录（github上指定的）
    - ~~gitbook serve~~ ~~生成目录前，需要把 docs 删除，不然目录里面会有这个，然后再执行 npm run build~~

- 报错
```text
报错1
Error: ENOENT: no such file or directory, stat 'C:\Users\lenovo\PycharmProjects\学习笔记\_book\gitbook\gitbook-plugin-sharing\buttons.js
关闭火绒软件（或者电脑管家、360等安全软件）就正常了，不需要重启开发者工具；

报错2
Template render error: (C:\Users\lenovo\PycharmProjects\学习笔记\Python\README.md) [Line 205, Column 14]
  unexpected token: }}

{{和}}之间加上空格变成{ {和} } （这里看不出区别，知道这个意思就行…） {%和%}之间加上空格变成{ %和% }


报错3
Error: ENOENT: no such file or directory, stat 'C:\Users\lenovo\PycharmProjects\学习笔记\_book\gitbook\gitbook-plugin-highlight\ebook.css'
再执行一遍 gitbook serve
```

- `mathjax`插件安装错误，[解决方法](https://zhuanlan.zhihu.com/p/132638228)
  - 首先安装`mathjax`，`npm install mathjax@2.7.7`
  - 接着在`book.json`中引入：
    ```json
    {
        "plugins": ["mathjax-pro"]
    }
    ```
  - 安装`gitbook install`


- [帮助链接](https://www.jianshu.com/p/0388d8bb49a7)
- [帮助链接](https://ldty.github.io/LearningJS/gitbook-editoran-88c52c-gitbook-bu-shu-dao-github-page.html)