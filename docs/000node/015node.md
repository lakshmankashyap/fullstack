### 更有用的场景

到目前为止，我们做的已经很好了，但是，我们的应用没有实际用途。

服务器，请求路由以及请求处理程序都已经完成了，下面让我们按照此前的用例给网站添加交互：用户选择一个文件，上传该文件，然后在浏览器中看到上传的文件。 为了保持简单，我们假设用户只会上传图片，然后我们应用将该图片显示到浏览器中。

好，下面就一步步来实现，鉴于此前已经对JavaScript原理性技术性的内容做过大量介绍了，这次我们加快点速度。

要实现该功能，分为如下两步： 首先，让我们来看看如何处理POST请求（非文件上传），之后，我们使用Node.js的一个用于文件上传的外部模块。之所以采用这种实现方式有两个理由。

第一，尽管在Node.js中处理基础的POST请求相对比较简单，但在这过程中还是能学到很多。 
第二，用Node.js来处理文件上传（multipart POST请求）是比较复杂的，它不在本文的范畴，但是，如何使用外部模块却是在本书涉猎内容之内。
