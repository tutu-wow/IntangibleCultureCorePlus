# IntangibleCultureCorePlus
非遗传承系统 亮点：WebSocket即时通讯、协同过滤算法推荐、支付宝沙盒支付、快递物流API、ECharts运营分析、微博与QQ链接分享、 非遗展示与互动、活动参与闭环、在线传习课程、 文创交易闭环； 角色：用户、传承人、管理员；

所有源码均本人开发，项目是前后端分离的，所有的项目都具备了完整的业务逻辑，不仅仅局限于基础的增删改查（CRUD）操作，系统亮点众多。

本文注重于计算机毕业设计选题指导，列出题目均有源码， 大家可以去【公众号】(毕业终点站)获取或者加我【qq】(2112698948)提意见(别忘记Star哟)。备注：git

声明：仅用于学习使用，请勿用于任何商业行为！

1.系统非商用，非开源，非无偿。

2.由本人开发，如需源码，请联系以下方式，qq:2112698948。

3.项目有很多，并未全部上传，如果未找到想要的，可直接咨询。

<div align="center">

# 非遗传承系统

**Spring Boot 3 + Vue 前后端分离 · 管理员 / 传承人 / 普通用户 三角色协作 45个表结构** 

非遗文化展示 · 传习课程 · 活动参与 · 文创交易

</div>

<p align="center"><img src="images/user-00-overview.png" width="100%"></p>

---

## 一、系统亮点

- 🎯 **协同过滤算法推荐**：根据用户参与活动的记录，找出兴趣相近的用户，推荐其尚未参与的活动，并补上热门活动；文化与视频内容同样带相关推荐，帮用户发现感兴趣的非遗内容。
- 💬 **WebSocket 即时通讯**：用户与后台之间提供在线聊天入口，消息通过 WebSocket 实时传递，方便沟通活动安排、课程学习和平台使用问题。
- 💰 **支付宝沙盒支付**：文创品订单与课程购买接入支付宝沙盒，支持完整的支付流程演示和订单支付状态查询，从下单到支付完成都能展示。
- 🚚 **快递物流 API**：接入第三方物流查询接口，按订单物流单号拉取轨迹并展示结果，用户可以跟进文创品的配送进度。
- 📤 **微博与 QQ 链接分享**：非遗视频、活动、课程和话题详情都可以一键分享到微博、QQ，把感兴趣的文化内容转给好友，扩大传播范围。
- 📊 **ECharts 图形化分析**：非遗项目数量、类型、覆盖地区、传承人数量和话题统计等图表，直观呈现文化资源分布和社区互动情况，方便管理员掌握平台数据。
- 👥 **三角色协作**：普通用户在线申请成为传承人，管理员审核资料，传承人通过工作台维护文化内容、课程、活动和文创品，把文化传播和业务运营连起来。
- 🏮 **非遗展示与互动**：整合非遗文化资料、传承人介绍、视频展览和话题交流，用户从了解文化、观看技艺到分享体验，形成持续互动。
- 📅 **活动参与全流程**：活动浏览、报名、审核、签到记录、活动评价都有对应页面，用户能随时跟进参与状态，后台也能管理活动记录。
- 🎓 **在线传习课程**：从课程预约购买到章节视频学习、进度记录、学习打卡和评价，帮助用户循序渐进地学习非遗技艺。
- 🛍️ **文创交易全流程**：传承人维护店铺、文创品和库存，用户完成收藏、加购、下单和支付，再通过订单、物流、评价与售后跟进交易。

---

## 二、技术选型

| 分类 | 技术 |
| --- | --- |
| 系统架构 | B/S、MVC、前后端分离、管理员 / 传承人 / 普通用户三角色管理 |
| 系统环境 | Windows |
| 开发环境 | IDEA、JDK 17、Maven、MySQL、Node.js |
| 后端技术 | Java、Spring Boot 3.3.1、Spring MVC、MyBatis-Plus、MySQL、JWT、WebSocket、支付宝 SDK、HanLP |
| 前端技术 | Vue、Vue CLI、Element UI、Vue Router、Vuex、Axios、ECharts、富文本编辑器 |

---

## 三、系统角色

| 角色 | 主要职责 |
| --- | --- |
| 普通用户 | 浏览非遗文化、查看传承人与影像、报名活动、购买与学习课程、逛文创商城、参与社区话题、在线咨询 |
| 传承人 | 申请审核通过后进入工作台，维护非遗文化、视频展览、活动、课程与文创品，处理库存和商家订单 |
| 管理员 | 审核传承人申请、管理非遗文化 / 活动 / 课程 / 传人 / 视频、处理用户咨询、话题管理与数据分析、发布系统通知 |

---

## 四、系统实现（核心截图）

### 4.1 用户端

<table>
  <tr>
    <td width="50%" align="center"><img src="images/user-01-home.png" width="100%"><br><b>首页</b></td>
    <td width="50%" align="center"><img src="images/user-02-heritage.png" width="100%"><br><b>非遗文化</b></td>
  </tr>
  <tr>
    <td width="50%" align="center"><img src="images/user-04-activity.png" width="100%"><br><b>非遗活动</b></td>
    <td width="50%" align="center"><img src="images/user-06-course.png" width="100%"><br><b>传习课程</b></td>
  </tr>
  <tr>
    <td width="50%" align="center"><img src="images/user-07-shop.png" width="100%"><br><b>文创商城</b></td>
    <td width="50%" align="center"><img src="images/user-09-video.png" width="100%"><br><b>非遗影像</b></td>
  </tr>
  <tr>
    <td width="50%" align="center"><img src="images/user-10-community.png" width="100%"><br><b>交流社区</b></td>
    <td width="50%" align="center"><img src="images/user-13-chat.png" width="100%"><br><b>在线聊天</b></td>
  </tr>
  <tr>
    <td width="50%" align="center"><img src="images/user-14-profile.png" width="100%"><br><b>个人中心</b></td>
    <td width="50%" align="center"></td>
  </tr>
</table>

用户端其余页面：非遗文化详情、活动详情、传承人物、交流详情、通知公告。

### 4.2 传承人端

<p align="center"><img src="images/inh-01-products.png" width="100%"></p>
<p align="center"><b>文创品维护</b></p>

<p align="center"><img src="images/inh-03-orders.png" width="100%"></p>
<p align="center"><b>商家订单</b></p>

<p align="center"><img src="images/inh-05-courses.png" width="100%"></p>
<p align="center"><b>课程列表</b></p>

<p align="center"><img src="images/inh-08-videos.png" width="100%"></p>
<p align="center"><b>视频展览</b></p>

传承人端其余页面：库存记录、非遗活动、课程订单、非遗文化。

### 4.3 管理员端

<p align="center"><img src="images/adm-01-consult.png" width="100%"></p>
<p align="center"><b>用户咨询</b></p>

<p align="center"><img src="images/adm-02-inheritor-audit.png" width="100%"></p>
<p align="center"><b>传承人申请审核</b></p>

<p align="center"><img src="images/adm-04-activity-record.png" width="100%"></p>
<p align="center"><b>非遗活动记录</b></p>

<p align="center"><img src="images/adm-06-topic-analysis.png" width="100%"></p>
<p align="center"><b>话题分析</b></p>

<p align="center"><img src="images/adm-12-notify.png" width="100%"></p>
<p align="center"><b>系统通知</b></p>

管理员端其余页面：非遗活动、话题信息、课程列表、课程订单、非遗文化、传人、视频展览。

---

## 五、关于本项目

本文档展示的是系统核心功能截图，完整源码、数据库脚本和部署说明不在仓库内展示。截图均存放于本地 `images/` 目录，不依赖外部图床。

如需了解完整功能、获取源码或定制开发，欢迎联系。

**文档展示 19 张截图，需要了解更多，请联系我。**
