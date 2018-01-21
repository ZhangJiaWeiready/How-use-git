#Git- 分布式版本控制器（Repository）
##linux命令
* mkdir xxx -- 新建文件夹
* vi xxx.xx -- 新建文件
	* i -- 进入编辑
	* esc ：wq  -- 保存并且退出
* cd xxx -- 进入xxx目录
* cd .. -- 返回上一目录
* ls -- 列出当前文件夹中所有的文件 
* pwd -- 显示当前目录
* cat x.txt -- 显示文件内容
* clear -- 清屏
##git的操作
* 基本操作
	* git init -- 初始化本地git库
	* git add */. --添加到暂存区
	* git commit -m ”“ -- 上传到版本区
	* git status -- 查看文件位置
	* git push -- 本地上传远程
	* git pull -- 远程下载到本地
* 查看提交版本
	* git log
	* git reflog
* 回退指定版本
	* git reset -- hard HEAD^ -- ^回退一个可叠加
	* git reset -- hard xxx -- xx版本号
	* git checkout -- xxx --撤销xxx版本的修改
* 删除指定文件
	* git rm xxx -- 删除xxx文件
	* git rm -r xxx -- 删除xx文件夹
* 分支操作
	* git checkout -b dev -- 创建dev分支
	* git branch 查看当前的分支
	* git checkout master 切换分支
	* git merge dev 合并指定dev分支到merge
	* git branch - d dev 删除指定分支
* 注意： 每个单词之间都需要用空格隔开
##远程/本地之间的操作
* 1. git pull 将远程新增改的文件拉到本地
* 2. git push 将本地上传到远程
* 3. git clone https/ssh 将远程库文件同步到本地库
##如何删除github中的文件
* find file -- 删除仓库中的单个项目
* setting delete --删除仓库
##
#本地远程交互
###本地仓库git （右键git bash）
* 1.新建文件夹把需要上传管理的文件放进去
* 2.git init -- 初始化git版本库（.git文件）
* 3.git add ‘.’/‘*’ -- 添加文件到暂存区
	* ！！！html文件名需改为index
	* 2.1 git status -- 查询文件现在所处的区域（绿色表示暂存区（stage）-add；红色表示工作区 - 未进行上传）
* 4.git commit -m “” -- 提交文件到版本库（主干master） ""-->描述
	* 3.1 git status --多次查询
* 5.git remote add origin xxx -- 将本地库与远程库连接
	* xxx表示gitbub的https/ssh的url
* 6.git push -u origin -- 将本地库内容同步到远程库中
	* “-u” 用于首次同步时，可忽略
### 远程仓库GitHub
* 1.新建仓库（new Repository）--create
* 2.![](https://i.imgur.com/jEznYfQ.png)
	* 点击setting
* 3.![](https://i.imgur.com/wyjcd34.png)
	* 点击none - 选择master branch - save 
* 4.![](https://i.imgur.com/wUhWsu9.png)
	* 复制https
* 5.![](https://i.imgur.com/XuA4n9Q.png)
	* 回到code - 选择edit - 粘贴url - save
* 6.可随时负值url查看内容









