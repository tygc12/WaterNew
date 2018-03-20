# README

## 介绍

UAP.SDK.Infrastructure

定义敏捷平台基础组件

**注意：**

本组件依赖 UAP.SDK.Share ≥ 1.0.0.0


## 更新记录

1. `2017-04-17`,【v1.0.0.1】

  * 增加Application、Container模块
  * 增加Logging模块


2. `2017-04-19`, 【v1.1.0.0】

  * 增加Caching 模块
  * 修改 IEntity 类型名称为 IEntityObject
  * 修改 ILogger 类型名称为 ILogProvider


3. `2017-04-19`, 【v1.3.0.0】

  * 增加Exception 管理模块

4. `2017-04-19`, 【v1.4.0.0】

  * 调整消息、事件处理模块接口定义

5. `2017-04-20`, 【v1.4.0.1】

  * 为 ExceptionManager、LoggerManager 两个类型增加 `sealed` 修饰，不允许继承。

6. `2017-04-21`, 【v1.5.0.0】

  * 增加 ILogProvider 的默认实现

7. `2017-04-21`, 【1.5.0.2】

  * 更新 SharpFrame.Commom 组件的版本到 1.0.0.2

8. `2017-04-21`, 【1.5.0.3】

  * 移除 JSONCacheProviderExtension.cs
  * 变更 MemoryCacheProvider 为 InMemoryCacheProvider

9. `2017-04-24`, 【1.5.0.4】

  * 重构ModelState中的BuildException方法，改为扩展方法。

10. `2017-04-24`, 【1.5.0.5】

  * 重构 ILogProvider 中IFormatProvider的传入顺序

11. `2017-04-24`, 【1.5.0.6】

  * 新增 ICacheProvider 的默认实现。作为其他缓存实现方案的基类

12. `2017-04-24`, 【1.6.0.0】

  * 重构 IObjectContainer接口以及默认实现。抽取类型注册为独立接口

13. `2017-04-25`, 【1.7.0.0】

  * 新增 Serialization 相关接口和多种默认实现。

14. `2017-04-26`, 【1.7.0.1】

  * 修复 DataObjects 命名空间错误问题

15. `2017-04-26`, 【1.7.0.2】

  * 调整 CacheProvider 中关于 Dispose 模式的实现方式

16. `2017-04-28`, 【1.7.0.3】

  * 新增多个 DataObject 定义:

    1. FaultData，WCF FaultContract 中异常信息
    2. AbstractResponseDataObject, 抽象的输出DataObject基类，定义Code，Message, Data等基本信息
    3. PageResultDataObject, 分页查询结果

  * 重命名 CacheProvider 为 AbstractCacheProvider
  * 修正部分命名空间不统一的问题

17. `2017-05-10`, 【1.7.0.5】

  * 解决 LogManager、ExceptionManage 不能使用的问题 

18. `2017-05-17`, 【1.8.0.0】

  * 重构部分抽象类的类名，增加Abstract前缀

	* AbstractObjectContainer
	* AbstractEntityObject
	* AbstractDomainEvent
	* AbstractLogProvider

  * 新增多个 AbstractResponseDataObject 子类。满足List、字典、Object、简单类型等多种情况的返回

19. `2017-05-17`, 【1.8.0.1】

   * 修复 AbstractResponseDataObject 类型中 Message 属性 类型定义错误问题。改为 String。
   * 为各种 AbstractResponseDataObject 子类增加构造函数
