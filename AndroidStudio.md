修改编码-->Generate-->Workspace
关联源码
libs\\file:android-support-v4.jar.properties
src=D:\\Win10ProgramFiles\\adt-bundle-windows-x86_32_20131019\\sdk\\extras\\android\\support\\v4\\src
ButterKnife
compile 'com.jakewharton:butterknife:7.0.1'
compile 'com.squareup.okhttp3:okhttp:3.5.0'
http://www.360doc.com/content/16/0106/22/20175734_526019813.shtml
http://blog.csdn.net/android_study_ok/article/details/51540759
https://8KLWRVG6PZKN85C/svn/RedBaby/trunk/code

   5.1 选项路径
   	5.1.1 File - Settings
   	5.1.2 File - Project Structure
   		可以修改SDK路径和Module依赖
   5.2 修改主题
	theme-->Appearance
   5.3 修改窗口字体
	
   5.4 显示内存占用
	mem-->Appearance-->show memory indicator
   5.6 版本更新
	updates
   5.7 显示建议行数提示(show right margin)
	margin-->Appearance-->show right margin
   5.8 显示行数
	margin-->Appearance-->show line numbers
reopen last
	reopen-->system settings-->reopen last project on startup
show quick documentation
	document-->general-->show quick documentation on mouse move 
   5.9 显示空白字符(换行、空格)
	white-->appearance-->show whitespaces
   5.10 代码自动补全提示
	case-->case sensitive completion-->none
	auto-->auto import-->choose all
   5.11 自动导包
	auto-->auto import
   5.12 设置代码字体
	font-->color&font
   5.13 文件编码
   	utf-8

6. 快捷键
   6.1 修改快捷键必须复制一份
   6.2 不建议映射为Eclipse快捷键
   6.3 资源查看
	6.3.0.1 ctrl+alt+s  打开设置
   	6.3.1 成员变量和成员方法跳转
   		ctrl + f12 --> alt + v
   	6.3.2 类跳转
   		ctrl + n
   	6.3.3 任意文件资源或设置项
   		双击 shift
   	6.3.4 跳转到下一个错误行
   		f2 --> alt + w
   	6.3.5 参数提示
   		ctrl + p
   	6.3.6 查看文档
   		ctrl + q	
		
		GBK + reload + utf-8 + Convert  GBK乱码
		
		alt + 1  打开project结构
		alt + 7  打开Structure结构
		ctrl + shift + 上下键     可以移动整个方法
		alt + shift + 上下键      向下移动一行
		ctrl + alt + m    抽取方法
		ctrl + alt + 左右键   移动到上次编辑的地方
		alt + 上下键  移到上一个方法	
		shift + F6  重命名
		ctrl + alt + F   局部变量提升为全局变量
		shift+鼠标滚动   编辑界面横向滚动
		ctrl + O  显示父类方法,重写方法
		Ctrl+Tab    打开界面切换窗口，保持按住Ctrl键，选中相应的要打开的窗口
		ctrl + w  选中,多次点击,范围扩大
		ctrl + shift + Enter   结束本行编辑,或跳转到下一行
		ctrl + shift + z   前进
		ctrl + z   	后退
		ctrl + alt + t    把选中的代码用常用的句式包起来
		ctrl + h	查看一个类的继承关系(Hierarchy)		
		method --> ctrl + 鼠标左键   显示方法被谁调用
		ctrl + shift + u --> 全部转为大写或小写
		ctrl + shift + 左右键 --> 选中当前光标左右两边的单词部分
		shift + 鼠标左键 --> 选中光标到鼠标点中位置的代码
		ctrl + r --> 替换
		ctrl + f --> 查找
		tab --> 修改方法时可与前一个方法重合
		

	自定义
		f2--> alt + w   跳转到下一个错误的位置
		ctrl + f4 --> alt + c   关闭当前编辑页面
		ctrl + f12 --> alt + v   成员变量和成员方法跳转
		alt + insert --> alt + g -->  generate  生成构造方法, setter getter 等
		shift + F10 --> alt + r --> 运行程序
		alt + b --> butterknife 生成
		alt + f --> gsonformat 生成
		alt + f7 --> alt + u -->  查看一个方法,变量,类等在一个工程的什么地方被使用
		alt + n --> 新建


   6.4 代码编辑
   	6.3 代码补齐(code - complition - base)
   		alt + / 
   	6.4 自动修复错误
   		alt + enter
   	6.5 格式化代码
   		ctrl + alt + L
   	6.6 复制选中行
   		ctrl + d
   	6.7 删除选中行
   		ctrl + y
   	6.8 剪切选中行
   		ctrl + x
   	6.9 自动删除未使用的包
   		ctrl + alt +ｏ
   	6.10 自动生成常用方法(getter、setter、构造等)
   		alt + insert
		ctrl + o  重写方法
	

7. 快速生成代码
   7.1 文件模板
   	editor - code style - file and code templates - include - file header

   	/**
   	*--------- 日期 ------- 维护人 ------------ 变更内容 --------		
   	*		2015.12.06		夏侯渊			新增Person类
   	*		2015.12.06		夏侯渊			增加sex属性
   	*/

   7.2 代码模板
   	7.2.0 editor - live templates
   	7.2.1 sout
   	7.2.2 fori
   	7.2.3 logt
   	7.2.4 fbc
   	7.2.5 loge
   	7.2.6 ctrl + j 显示代码模板提示
	logm
	const
	.var
	.try
	.field
	

8. 插件
   8.1 MarkDown
   8.2 WifiAdb
	adbcommander

9. Debug调试

10. TestCase测试

11. Gradle
    11.1 %project%/settings.gradle
    	声明项目里所有的模块

    11.2 %project%/build.gradle
    	11.2.1 jcenter()
    		源码仓库，如果下载jar包总是失败，可以尝试替换为 mavenCentral()
    	11.2.2 dependencies
    		gradle插件版本，一般与AndroidStudio版本相同。

    11.3 %module%/build.gradle
    	项目的编译脚本，包含应用使用的SDK和应用版本信息，以及依赖的第三方库等配置

    11.4 提供Gradle文档·
    	建议使用百度

12. AS新建和导入项目
    12.1 新建项目。
    	12.1.1 Project(项目) --> Eclipse的Workspace(工作空间)
    	12.1.2 要支持5.0新特性，使用API21版本
    12.2 新建模块
    	12.2.1 Module(模块) --> Eclipse的Project(项目)
    12.3 导入项目
    	12.3.1 随便准备一个AS项目用于展示
    	12.3.2 存在build.gradle则说明是AS项目
    12.4 导入模块
    	12.4.1 提前准备一个Utils包用于展示
    	12.4.2 
    	存在settings.gradle则说明是项目，不存在则说明是模块的代码
    12.5 项目依赖
    	12.5.0 File - Project Structure - app - Dependence - add
    	12.5.1 Libary Dependency
    		添加Maven库，直接从网络下载第三方库
    		示例 fastjson、xutils
    	12.5.2 File Dependency
    		添加jar包
    		示例 任意jar包
    		注意：直接粘贴到libs目录也可以，但是需要手动重新sync
    	12.5.3 Module Dependency
    		关联Module
    		示例，关联一个Utils的Module
    	12.5.4 图形界面的关联，实际上最终是在build.gradle里添加配置
    12.6 删除项目、模块
		12.6.1 删除项目只要删除项目文件夹就可以
		12.6.2 删除模块需要在 settings.gradle 里去掉模块，然后在项目上右键删除

13. 导入Eclipse项目
    13.1 导入项目
    	13.1.1 网上的导入方法很多，最新版的AS直接在ImportProject时选中Eclipse项目即可生成AS结构的项目
    	13.1.2 想要保持原先的Eclipse目录结构，则需要使用最新的Eclipse和ADT插件，生成gradle文件。
    		13.1.2.1 生成的gradle文件需要修改使用的gradle插件版本
    		13.1.2.2 生成的gradle文件夹需要删除掉
    13.2 导入模块
    	直接import module

