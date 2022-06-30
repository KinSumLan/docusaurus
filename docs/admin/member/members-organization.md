---
title: 管理组织架构成员 - CODING 帮助中心
pageTitle: 管理组织架构成员
pagePrevTitle: 管理组织架构
pagePrev: admin/member/organization.html
pageNextTitle: 通过企业微信导入成员
pageNext: admin/member/wecom.html
---

利用「团队设置中心」->「全局设置」->「组织与成员」->「成员管理」中的组织架构功能创建部门/子部门或从[企业微信](/docs/admin/member/wecom.html)、[腾讯云](/docs/admin/member/cloud.html)或 [LDAP](/docs/admin/member/ldap.html) 导入成员/部门数据之后，可将成员归类到不同部门实现有序管理。

![](https://help-assets.codehub.cn/enterprise/20220412143808.png)

通过不同的应用添加成员之后，能对组织架构成员执行的操作有所差异。如下表所列，若通过企业微信或 LDAP 导入成员数据，将不能修改导入成员的部门或删除成员。对于从 CODING 平台直接添加的用户，不涉及授权或关联已有成员操作。

|         操作 | CODING | 企业微信 | 腾讯云 | LDAP | LDAP（不带 ou） |
| :----------- | :----- | -------- | ------ | ---- | --------------- |
|     查看用户详情 | ✅     | ✅       | ✅     | ✅   | ✅              |
|   关联用户组 | ✅     | ✅       | ✅     | ✅   | ✅              |
|       重命名成员 | ✅     | ✅       | ✅     | ✅   | ✅              |
|     添加成员至部门 | ✅     |          | ✅     |      | ✅              |
|         删除成员 | ✅     |          |        |      |                 |
|         授权成员 |        | ✅       | ✅     | ✅   | ✅              |
|     取消授权 |        | ✅       | ✅     | ✅   | ✅              |
| 关联已有成员 |        | ✅       | ✅     | ✅   | ✅              |


### [查看成员详情](#view)

在组织架构列表，点击成员姓名，会显示部门成员详情页。在该成员的详情页面，你可以为其指定团队角色以及在具体项目内的角色。


### [关联用户组](#allocate)

部门成员支持设置用户组操作。设置了对应用户组之后，该成员即拥有对应用户组的相关权限。阅读[权限配置](/docs/admin/permission.html)了解如何划定用户组权限。

![](https://help-assets.codehub.cn/enterprise/20210929160017.png)


### [重命名成员](#rename)

部门成员支持重命名操作，可修改不符合团队命名规范的成员名称。重命名成员不会修改该成员在第三方服务中显示的姓名。

![](https://help-assets.codehub.cn/enterprise/20210929160104.png)

### [添加成员至部门](#set-department)

一个成员可设置多个不同的部门归属，当取消成员所有部门设置之后，部门成员将自动设置到根部门下。

> 设置部门操作支持批量处理。可点击部门成员列表右下角的「批量处理」，勾选成员，再点击左下角「设置所在部门」进行批量设置。

![](https://help-assets.codehub.cn/enterprise/20210929160104.png)


### [授权成员](#authenticate)

第三方应用导入成员需获得授权后才可以访问 CODING。点击「授权」，弹出授权确认弹窗，点击确认按钮即可。

![](https://help-assets.codehub.cn/enterprise/20210929160332.png)

授权后用户变成已授权状态，也会在第三方平台收到通知。该成员需登录或注册 CODING 账号后才能加入团队，变成**已加入**状态。

> 团队成员的授权状态说明如下：
> -   **未授权**：（只针对第三方导入成员）该成员无权访问 CODING。
> -   **已授权**：（只针对第三方导入成员）该成员有权访问 CODING，但尚未加入团队。成员需登录或注册 CODING 账号并加入团队之后才能在 CODING 平台进行操作。
> -   **已加入**：该成员已通过邀请链接登录或注册 CODING 账号，并且加入了该团队，能在团队内进行相应操作。

### [取消授权](#cancel)

第三方应用导入成员可被取消授权。取消授权后，成员将无法访问 CODING 服务并处于未授权状态。

![](https://help-assets.codehub.cn/enterprise/20210929160541.png)

### [关联已有成员](#associate)

如果通过第三方应用导入的成员已经是 CODING 成员，可在该用户的详情页面将其与已有的 CODING 成员进行关联。关联后该成员的历史数据会保留并变成已加入状态。

![](https://help-assets.codehub.cn/enterprise/20210929162332.png)

### [一键匹配](#map)

通过第三方应用导入的部门成员支持一键匹配功能。可通过用户姓名、邮箱、手机等信息，将无法自动关联的用户进行关联，也可按需调整第三方用户与 CODING 用户之间的关系。

![](https://help-assets.codehub.cn/enterprise/20210929162542.png)
![](https://help-assets.codehub.cn/enterprise/20210929162615.png)


### [删除成员](#delete)

此操作支持删除成员，点击成员更多操作触发。若成员存在未交接事件，会弹出提示前往交接页面。

> 删除成员操作支持批量处理。可点击部门成员列表右下角的「批量处理」，勾选成员，再点击左下角「删除」完成批量删除。

![](https://help-assets.codehub.cn/enterprise/20201117192548.png)

### [常见问题](#ban)

**如何保证企业微信通讯录中的成员删除之后自动离开 CODING 团队？**

你可以使用成员自动同步功能实现该目的。有关详细操作信息，请参考[成员自动同步](/docs/admin/member/wecom.html#sync)。

