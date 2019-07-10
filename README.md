# The Test Ground for seeleteam.js
总原理是: 
fork seeleteam.js 后clone到本地修改
- 修改后把seeleteam的package.json的name改成seeleteamme.js和version改成符合个人账户下的prototype的名称和版本号
- 在该文件夹中npm login个人账户, npm publish
- clone 这个repo下来, 在try.js里 var seeleteam = require('seeleteamme.js')
- 在tg里npm install然后 node try.js来测试效果(gitignore了package.json所以每次都会下载最新的seeleteamme)

如果测试效果可以, 回到seeleteam.js
- 改动确认, 复原package.json里的修改
- git add, git commit, git push, pull requests
- clone公司repo里的seeleteam.js下来npm login个人账户, npm publish