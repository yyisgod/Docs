#git reset --hard <commit_id>

#git push origin HEAD --force

##
有时候对源文件做了点修改，也已经commit了，又不想要这个修改了怎么办？
可是你用的事master分支啊，没法删的啊。

这时候就要用上面这两个命令来回到你之前的一个commit状态了。

commit_id就不用说了，很容易就可以找到。
用法如下：

	git reset --hard <commit_id>
	git push origin HEAD --force
执行了这两条命令就会退回之前的状态了。

注意`reset`后不要忘了`push`啊

##其他
根据`–soft –mixed –hard`，会对working tree和index和HEAD进行重置:

    git reset –mixed：此为默认方式，不带任何参数的git reset,即时这种方式，它回退到某个版本，只保留源码，回退commit和index信息
    git reset –soft：回退到某个版本，只回退了commit的信息，不会恢复到index file一级。如果还要提交，直接commit即可
    git reset –hard：彻底回退到某个版本，本地的源码也会变为上一个版本的内容


    HEAD 最近一个提交
    HEAD^ 上一次
    <commit_id>  每次commit的SHA1值. 可以用git log 看到,也可以在页面上commit标签页里找到.