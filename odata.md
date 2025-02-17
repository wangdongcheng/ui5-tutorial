正如本教程的开篇介绍文章[SAP OData 开发教程 - 从入门到提高(包含 SEGW, RAP 和 CDP)](https://jerry.blog.csdn.net/article/details/125468125)所提到的，SAP OData 服务开发，从实现技术上来说，可以分为三大类。因此本教程也分为三大部分，分别进行介绍。本文是本教程的文章目录。

## 作者简介

Jerry Wang，2007 年从电子科技大学计算机专业硕士毕业后加入 SAP 成都研究院工作至今。Jerry 是 SAP 社区导师，SAP 中国技术大使。在长达 15 年的 SAP 标准产品开发生涯里，Jerry 曾经先后参与 SAP Business ByDesign, SAP CRM, SAP Cloud for Customer, SAP S/4HANA, SAP Commerce Cloud(电商云)等标准产品的研发工作。

Jerry 对 SAP OData 服务的开发，测试，发布，部署，测试，及基于各种不同 SAP 技术实现的 OData 服务的幕后技术实现细节和使用场合，均有着深入的研究。

![](https://img-blog.csdnimg.cn/ac9f815e59e34b1088e3bb0802622fb9.jpeg#pic_center)

# 基于 SEGW - Gateway Service Builder 的开发教程

- [0. SAP 标准产品里使用 OData 服务的一些细节分享](https://jerry.blog.csdn.net/article/details/127593757)

- [1. 在 SAP ABAP 事物码 SEGW 里创建 SAP OData 项目](https://jerry.blog.csdn.net/article/details/125768423)

- [2. 在 SAP ABAP 系统对事物码 SEGW 创建的 OData 服务进行配置并测试](https://blog.csdn.net/i042416/article/details/125781692)

- [3. SAP ABAP OData 服务诊断工具 /IWFND/ERROR_LOG 的使用方法](https://jerry.blog.csdn.net/article/details/126054502)

- [4. SAP ABAP OData 服务 Data Provider Class 的 GET_ENTITYSET 方法实现指南](https://blog.csdn.net/i042416/article/details/126062166)

- [5. SAP ABAP OData 服务如何支持 $filter (过滤)操作](https://blog.csdn.net/i042416/article/details/126079417)

- [6. 使用 Postman 工具高效管理和测试 SAP ABAP OData 服务](https://jerry.blog.csdn.net/article/details/126084987)

- [7. SAP ABAP OData 服务如何支持 $orderby (排序)操作](https://jerry.blog.csdn.net/article/details/126089889)

- [8. SAP ABAP OData 服务如何支持创建(Create)操作](https://jerry.blog.csdn.net/article/details/126096205)

- [9. SAP ABAP OData 服务如何支持删除(Delete)操作](https://blog.csdn.net/i042416/article/details/126108785)

- [10. SAP ABAP OData 服务如何支持修改(Update)操作](https://blog.csdn.net/i042416/article/details/126130059)

- [11. 使用 HTTP PUT, PATCH 以及 MERGE 请求消费 SAP ABAP OData 服务修改操作的实现及其区别](https://jerry.blog.csdn.net/article/details/126142762)

- [12. SAP ABAP OData 服务如何支持 $select 有选择性地仅读取部分模型字段值](https://jerry.blog.csdn.net/article/details/126163273)

- [13. SAP ABAP OData 服务的分页加载数据集的实现(Paging)](https://blog.csdn.net/i042416/article/details/126191715)

- [14. 几种 SAP ABAP OData 服务的性能评估和测试工具介绍](https://blog.csdn.net/i042416/article/details/126196909)

- [15. SAP ABAP OData 服务里 EntityType 和 EntitySet 的区别](https://jerry.blog.csdn.net/article/details/126383625)

- [16. 如何修改 SAP ABAP OData 模型，使其支持 $expand 操作](https://jerry.blog.csdn.net/article/details/126402523)

- [17. 如何通过 SAP ABAP OData $expand 操作在同一个 HTTP 请求中返回多个节点的数据](https://jerry.blog.csdn.net/article/details/126445641)

- [18. SAP ABAP OData 服务嵌套创建功能的实现步骤(Create Deep)](https://jerry.blog.csdn.net/article/details/126601507)

- [19. 如何使用 ABAP 程序消费 SAP ABAP OData 服务](https://jerry.blog.csdn.net/article/details/126613213)

- [20. 如何使用 ABAP 代码消费需要传递 CSRF token 的 OData 服务](https://jerry.blog.csdn.net/article/details/126718687)

- [21. SAP ABAP OData 服务的 $count 操作实现](https://jerry.blog.csdn.net/article/details/126921513)
 
- [22. SAP ABAP OData 服务的 $count 和 $inlinecount 两个操作的区别](https://blog.csdn.net/i042416/article/details/126924558)

- [23. 如何给 SAP ABAP SEGW 开发的 OData 服务添加 Access-Control-Allow-Origin 响应头](https://jerry.blog.csdn.net/article/details/127188171)

- [24. SAP 标准产品里使用 OData 服务的一些细节分享](https://blog.csdn.net/i042416/article/details/127593757)

- [25. 答疑 - SAP OData 框架处理 Metadata 元数据请求的实现细节，前后端组件部署在同一台物理服务器](https://jerry.blog.csdn.net/article/details/128158298)

- [26. SAP ABAP OData Gateway 框架里 /IWFND, /IWBEP 这些缩写代表了什么含义？](https://jerry.blog.csdn.net/article/details/128178945)

- [27. SAP OData 框架里的缓存(Cache)设计专题讲座](https://jerry.blog.csdn.net/article/details/128365532)

- [28. 如何使用 SAP OData 服务向 ABAP 服务器上传文件](https://jerry.blog.csdn.net/article/details/128405227)

- [29. 如何通过 ABAP 代码给 SAP OData 元数据增添注解](https://jerry.blog.csdn.net/article/details/128411994)

- [30. 如何使用 SEGW 的 redefine 功能对 SAP 标准 OData 服务进行扩展](https://jerry.blog.csdn.net/article/details/128516573)

- [31. SAP UI5 Fiori 应用在启动时向 ABAP 后台发起的 OData 请求序列的顺序和作用分析](https://jerry.blog.csdn.net/article/details/128575198)

- [32. 关于 Fiori 应用里 SAP UI5 前端开发和 SEGW 后台 OData 服务开发的工作量比值问题](https://jerry.blog.csdn.net/article/details/128939305)

- 更多文章正在写作中，敬请期待

# 使用 Restful ABAP Programming 编程模型(简称 RAP) 开发 OData 服务

- 正在写作中，敬请期待

# 使用 SAP Cloud Application Programming 编程模型开发 OData 服务

* [1. SAP Business Application Studio 里创建一个基于 CAP 模型的最简单的 OData 服务](https://blog.csdn.net/i042416/article/details/128058748)

* [2. 如何给在 SAP Business Application Studio 里开发的 OData 服务准备测试数据](https://blog.csdn.net/i042416/article/details/128063472)

- 正在写作中，敬请期待