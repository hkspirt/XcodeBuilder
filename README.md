XcodeBuilder
===============

功能：一键打包IPA
起因：项目通过svn协作开发，只有一台Mac，每次打包都得重新拖代码和资源文件。十多个平台
      操作相当麻烦。
      
实现思路：
1、shell更新svn的代码和其他资源
2、根据规则修改xcode工程文件
3、shell生成ipa并提交svn

xcode工程文件操作基于：https://github.com/jasperblues/XcodeEditor
(增加了对.c和folder的支持，屏蔽部分写文件操作等...)

待完善：
1、部分路径和屏蔽文件改成读取配置，现在是写死的
2、oc不会,边百度边写的,神马内存释放，空指针都没管...
3、怎么生成可执行文件啊...?

有什么更好的办法求指导...