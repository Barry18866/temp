Markdown,文本修饰语言，用特殊符号修饰正文效果<br>

## 标题修饰符\#

# 标题修饰符(一级标题)
## (二级标题)
### (三级标题)
#### (四级标题)
##### (五级标题)


## 正文内容
  输入正文内容，但是如果需要换行，用\<br\> 标签

## 修饰正文
   *一段测试文本*
   
   **一段测试文本**
   
   ***一段测试文本***
   
   ~~一段测试文本~~

##分割线

  用\-\-\- 表示分割线
 
---

## 引用效果\>表示
> 你自己就是一座金矿，关键在于如何挖掘和利用自己
>> 四个拉低
>>> 三级引用
>>>> 四级引用

##列表
### 无序列表 \*
* 二次元
  * 原神
    * 神里绫华
  * 大逃杀类
    *PUBG
    *APEX

### 有序列表 1.
1. 物理学
   1. 粒子物理
   2. 原子核物理
   3. 凝聚态物理
2. 计算机科学
   1. 分布式架构
   2. 云计算
### 混合列表
1. 测试一级
   * 测试二级 
   2. 测试三级

## 表格
名称|技能|排行
--|:--:|--:
蝙蝠侠|有钱|32
海王|游泳|16
闪电侠|跑|18

### 代码片段

```c
	#include <stdio.h>
	int main(void)
	{
		printf("test code\n");
		return 0;
	}

```

```cpp
	#include <iostream>
```
```python
	import <os>
```
```bash
	echo "测试"
	pwd
	ps aux
	ls -l
```
   这是一段测试文本，将`关键字`，重点显示

### 超链接技术


[https://github.com/Barry18866/temp?tab=readme-ov-file](https://github.com/ "点击访问")


### 插入图片

![壁纸图片](C://Users//dell//Deskto//1.png "悬停标题")


---
#**2-3节课笔记**

**关键字查询** awesome,去此标签类别中查询项目
	       Python tutorial 查询资料，书籍，文档
	       socket sample 查询对应技术的代码样本

## **Github 三要素**

1. **仓库**
   1. 仓库是github的项目管理单元，每个用户都可以创建属于自己的仓库将项目代码资源传到仓库中保存项目传到github中可以云存储 保存与备份
   2. 一个用户是可以有多个仓库
   3. 便于分享，可以通过https连接分享仓库数据
####**code** 
   4. 工程资源，包含代码，资源数据，库，许可证，阅读文档等等
####**issues**
	问答标签
####**README.md** 
	工程的自述文件，使用markdown语言编写
####LICENSE 许可证 
	*GPL3.0* *MIT* *APCHE2.0* *BSD*

2. **提交**
   1. 用户在上传代码时可以通过提交来备份代码信息
   2. 提交可以备份代码片段，并且统计展示用户的修改
   3. 可以通过提交记录，回溯任意代码片段
   4. 提交可以记录开发的详细过程（文件的创建及代码的修改）

3. **分支**
   1. 资源存储唯一单位，用户存储代码数据等等，一个仓库是由若干分支构成
   2. 每个仓库创建后都有一个默认的主分支，代码上传都存储在分支中
   3. Master/Main（默认主分支）
   4. 多人协作开发

---

## **语法**

**git init** 创建本地仓库 ps：*仓库是隐藏数据*、
**git add filename** #*将数据资源添加到git缓冲区*
**git restore filename** #*将本地删除的文件还原 仓库中有备份* 
**git rm filename** #*不仅删除本地，也删除本地仓库，无法还原*
**git status** #*查看缓冲区*

**git commit -m "一次提交"** #*-m 后加标注*

**git push origin master** #*将本地分支上传到云端，如果分支相同则合并，否则，云端创建新分支，保存上传内容*

**git pull** #*如果云端内容更新，可以把云端仓库数据拉到本地*

**git clone https的项目地址** #*克隆项目的内容到本地*

**git pull rebase origin master**#*如果云端仓库数据与本地不一致，可以先拉取更新再推送*

**git rebase --abort** #*忽略新版*

**git rebase --skip** #*忽略旧版*

**git rebase --continue** #*版本合并*

### **完成账号绑定（关联）**
     1.git config --list #*查看本地配置文件*
     2.git config --global user.email = 注册邮箱
     3.git config --global user.name  = 账户名

### 此命令在config配置中添加或修改配置项

    1. ssh-keygen -t rsa -C "注册邮箱" //*创建本地密文*

    2. ssh -Tgit@github.com #*测试关联是否完成*

    3. c/user/用户名/.ssh/id_rsa.pub 复制密文，粘贴到账户中
   **Settings->SSH and GPG keys->new SSH keys->粘贴**

### 目标仓库设置别名，创建一个云端仓库的地址别名
    * git remote add origin git@github.com:Barry18866/20230715.git #*生成SSH地址别名 origin是地址别名*
    * git remote remove origin # *删除地址别名*





