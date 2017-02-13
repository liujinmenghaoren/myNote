#.gitignore
在git项目管理中会遇到这样的情况，把没有必要的和不想上传的文件／文件夹。上传到了的代码仓库。想避免这个尴尬很简单，

### .gitignore 文件的使用步骤
- 打开 git bash；
- 输入 touch .gitignore  
//创建.gitignore 隐藏文件  

- vim .gitignore        
//编辑  .gitignore 文件，加入想要忽略的文件。

如图所示：

![ignore](../img/ignore.png)

- 如果添加 .gitignore 文件之前已经添加想要忽略的文件，那么后来添加的 .gitignore 文件时无法对之前添加的文件起作用的。那么怎么办呢？可以这样：
  - git pull [] []
  - git rm -r --cached .
  - git add .
  - git commit -m ""
  - git push [] []


- vim 编辑文件的语法：
  - 修改
      - :i  进入编辑状态
      - i   在光标当前位置向前插入
      - I   在本行第一个字符前插入
      - a   在光标当前位置向后插入
      - A   在本行末尾插入
      - o   向下插入一行
      - O   向上插入一行
      - :w  保存
      - :q  退出
      - :wq 保存并退出
  - 删除
      - x   删除当前字符
  	  - dd  删除当前行
  	  - dw  删除当前光标下的词
  -复制粘贴
      - yy  复制当前行
      - yw  复制当前光标下的词
      - p   粘贴
      - p   粘贴在当前位置之前
      
