## 同步svn版本文件至测试环境

在开发过程中，一般会出现从开发环境部署至测试环境，有时不是简单的一个`svn up`就能解决。最近新项目中也出现这样的情况（为什么没有公司的部署体系支持？因为总有些爷），于是迅速弄了一个可快速更新文件至测试环境的小工具。

**要求**：
- 基于svn是分支开发
- 测试环境的php所属用户有svn操作权限。

**功能**：
- 支持从指定分支中的指定文件更新至测试环境

**to do list**:
- 更新指定文件的指定版本，如file 1234
- 命令工具，实现up2test [-r 1234]，更新提交版本至测试环境（默认最新一个版本）