# README

## 介绍

UAP.SDK.Infrastructure.Storage.EntLib

数据访问组件，基于企业库 DAAB 组件。

**注意：**

本组件依赖：

SH3H:

  * UAP.SDK.Infrastructure ≥ 1.8.6.1
  * UAP.SDK.Share ≥ 1.0.0.3
  * SH3H.SharpFrame.Common >= 1.0.1.5

第三方:

  * EnterpriseLibrary.Common, 6.0.1304.0
  * EnterpriseLibrary.Data, 6.0.1304.0


## 更新记录

1. `2017-04-21`,【1.0.0.0】

  * 初始版本

2. `2017-12-14`, [1.0.10.0]

  * 为BaseDataAccess<TEntity>类型增加 SelectSingle 系列方法
  * 重构BaseDataAccess._PrintCommandText方法，尽在允许Debug日志输出时输出日志
