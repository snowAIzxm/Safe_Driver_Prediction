小组说明 
1）获取源码分支 首先登录github网站fork https://github.com/liuqiaoping7/Safe_Driver_Prediction.git。 
   本地git clone https://github.com/自己的用户名/Safe_Driver_Prediction.git。 
2）本地编辑，push代码到自己的fork分支 git add --all git commit -m "application for.." git push origin master 
3）分支同步 
    (1).组员push request之前，需要先从组代码pull最新的代码并合并测试通过： 
        常用几条命令： 
        git remote add upstream https://github.com/liuqiaoping7/Safe_Driver_Prediction.git (添加组内公共源) 
        git remote -v (查看 是否添加成功) 
        git checkout -b source (新建一个分支,名称任意) 
        git pull upstream master (分支与组内源同步) 
        git checkout master (回到master分支) 
        git merge source (合并source到master分支，merge只解决文件内容合并，自动合并冲突部分手动修改，逻辑冲突部分测试后发现) 
        git add * (若有手动修改，需要添加到工作区) 
        git commit -m "merge for.." (若有手动修改，生成新的节点) git push origin master (提交到github) 
    (2).发起pull request，在github上网页操作。 
    (3).组长merge组员的贡献到origin/master。 
4）回退操作：
    git reset --hard HEAD (恢复到最近一次提交) 
    git checkout -- file (或者丢弃单个文件修改就是) 
    git clean -dxf (则会丢弃所以没有add的修改，保持工作区的清净) 基本上这些命令就差不多够了. 
如果希望系统了解git，可看看廖雪峰的教程：百度网盘 http://pan.baidu.com/s/1eSkHTrc 提取码 dagu. 
