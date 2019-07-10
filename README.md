# The Test Ground for seeleteam.js
总原理是: 

fork seeleteam.js 后clone到本地修改
- 修改后把seeleteam的package.json的name改成seeleteamme.js
- 统一文档内把version改成符合个人账户下的prototype的版本号
- 在该文件夹中npm login个人账户, npm publish

用tg来测试这个npm包的效果

- clone 这个repo下来, 在try.js里 var seeleteam = require('seeleteamme.js')
- 在tg里修改package.json到版本号至当前prototype版本号, npm install然后 
- 端口跑 node try.js来测试效果

如果测试效果可以, 回到seeleteam.js
- 改动确认, 复原package.json里的修改
- git add, git commit, git push, pull requests
- clone公司repo里的seeleteam.js下来npm login个人账户, npm publish