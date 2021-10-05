<h1 style="text-align:center"> Dos命令 </h1>	

### Dos介绍

> Disk operating System 磁盘操作系统。

```javascript
// 在E盘创建一个newdir目录(make dir)
1.md E:\\newdir
// 移除E盘newdir目录（remove dir）
2.rd E:\\newdir
// 查看当前目录下所有目录
3.dir  
//切换到其他磁盘
//示例切换到F盘，/D是固定的
4.cd /D f: 
//切换到当前盘其他目录
//当前目录E:\\JuLianWork
5.1 cd hss  // 当前目录E:\\JuLianWork\hss
5.2 cd ../data  //当前目录E:\\data
5.3 cd /    //切换到根目录
// 生成当前目录下的所有目录树
6.tree
//清屏
7.cls
//退出
8.exit
** 非重点 **
//在当前目录下的为mogen.txt编辑内容
9.E:\JavaWorkSpace> echo 晚上好 >mogen.txt
//拷贝文件
E:\JavaWorkSpace>copy mogen.txt e:\zs.txt  //将当前目录下的mogen.txt拷贝到E盘下的zs.txt中(不指定文件名则会赋值一个同名文件)、、
//剪切文件
10.E:\JavaWorkSpace>move mogen.txt F:
```

