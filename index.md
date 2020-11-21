崔洛崎
201812155003
- UML作业
- 用例名称	GitHub System
用例说明	Adminstrator在登陆后可以进行添加文件、设计专案、下载源代码、查看文件、设置安全策略等操作。  
User在登陆后可以进行查看文件、添加文件、下载源代码等操作。
参与者	Adminstrator、User  
元素	Add File、Projects、Download Code、Go To File、Security System  
关系	Adminstrator对于Add File、Projects、Download Code、Go To File、Security System是依赖关系
User对于Add File、Download Code、Go To File是依赖关系
建模思路	1.Administrator和User当登录GitHub之后可以进行查找和修改文件  
参与者Administrator可直接对文件进行修改，还可以查看其他用户对此文件的修改请求并进行审批。同时Administrator还可以在仓库中设计专案并对仓库中文件设置安全策略等  
2.参与者User 可以查找文件并提出对该文件的修改请求，等待项目管理员的审批  

- 用例名称	Add File
用例说明	User和Administrator向项目中添加或更新文件
参与者	Adminstrator、User
元素	Create new file、Upload files、Commit new file、Commit new file、Commit directly、Create a new branch、Commit directly、Create a new branch
关系	Administrator和Userr对于Add File用例是关联关系
Create new file、Upload files对于Add File是包含关系
Commit new file对于Create new file是包含关系
Commit new file对于Upload files是包含关系
Commit directly、Create a new branch对于Commit new file是包含关系
Commit directly、Create a new branch对于Commit new file是包含关系
建模思路	1.在Add File的功能操作下，User和Adminstrator均有对文件修改并在仓库中创建新文件的操作
2.在Commit new file的功能操作下，User和Adminstrator都有两种提交操作：直接提交和创建一个新的分支提交
