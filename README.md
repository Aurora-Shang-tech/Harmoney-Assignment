# 同行小队 · 团队课程网站

双击 index.html 打开团队首页。纯 HTML5 + CSS3，无需安装依赖或编译。城市图片已存入项目，离线可显示；访问外部资料需联网。

## 页面结构

- index.html：团队首页，四位成员入口、合肥城市介绍、内嵌 CSS 与多处行内 CSS。
- personal.html：商徐炜的个人主页，学号 SA26225270。
- skills.html：商徐炜的职业技能页面。
- members/member-2/index.html 与 skills.html：第二位成员的两个预留页面。
- members/member-3/index.html 与 skills.html：第三位成员的两个预留页面。
- members/member-4/index.html 与 skills.html：第四位成员的两个预留页面。
- team.html：兼容原团队链接，自动前往 index.html。
- css/style.css：页面共用的外部样式。
- images/hefei-swan-lake.jpg：合肥天鹅湖城市照片。
- images/favicon.svg：标签页图标。

目前只有商徐炜的真实资料，另外三位成员使用明确标注的占位信息，不代表真实姓名或学号。团队首页 + 四位成员各两个页面，共九个内容页，另有一个旧链接兼容页。

## 后续接入其他成员

1. 在 index.html 的成员卡片中填写真实姓名与学号，替换 MEMBER_2_STUDENT_ID、MEMBER_3_STUDENT_ID、MEMBER_4_STUDENT_ID。
2. 填写对应 members/member-N/ 目录里的 index.html 和 skills.html，替换标题、姓名、学号及待补充内容。
3. 如果已有成员网站，可将其两页接入相应目录；仍使用 index.html、skills.html 时无需修改团队首页链接。若采用其他路径，请同步修改成员卡片的 href。
4. 子目录引用共用样式和图片时，使用 ../../css/style.css 与 ../../images/；返回团队首页使用 ../../index.html。
5. 全部接入后，将团队介绍中的“目前已接入 1 位成员，其余 3 位资料待补充”更新或删除。
6. 商徐炜本人照片仍需放入 images/profile.jpg；未提供时显示姓名占位。

已按最新要求移除联系区域、邮箱入口和介绍视频，无需补充邮箱或视频。

## 团队首页考核对照

| 要求 | 实现 |
| --- | --- |
| 第一个页面为团队页面 | index.html |
| 成员姓名、学号、个人主页链接 | 四张成员卡片；商徐炜已填写，其余三位待提供真实资料 |
| 每位成员两个页面 | 一位完整内容 + 三位各自的个人主页和职业技能模板 |
| 城市介绍五项内容 | 合肥：地理位置、人口、风景名胜、文化、美食 |
| 城市图片与图片超链接 | 本地天鹅湖照片，点击前往政府网站城市介绍 |
| 更多信息外部链接 | 城市概况、人口数据、古镇文化、美食线路 |
| 内嵌自定义 CSS | index.html 的 head 内 style 标签 |
| 共用选择器 | h1, h2, h3 |
| 类选择器 | .member-card、.team-intro 等 |
| 上下文选择器 | .member-card p、.city-photo figcaption 等 |
| a 标签 hover | .team-page a:hover |
| 多处行内 CSS | 团队副标题、介绍、成员概况、人口卡片等 |
| 响应式 | 1024px、768px 媒体查询，成员卡片四列／两列／单列 |

商徐炜的个人主页保留外部 CSS、内部 ID/标题/上下文选择器、教育经历、项目、职业规划及游戏／电影／旅行兴趣。职业技能页保留硬技能、软技能、学习路线与六处行内 CSS。

## 城市资料与图片来源

人口使用有明确统计年份的数据：2024 年末合肥全市常住人口 1000.2 万人，不表述为实时人口。

- 城市概况：https://www.hfyaohai.gov.cn/tzyh1/zszy/11281847.html
- 人口数据：https://www.ahhuoshan.gov.cn/public/6597881/38582813.html
- 古镇与文化：https://www.mct.gov.cn/whzx/qgwhxxlb/ah/201909/t20190924_847008.htm
- 美食线路：https://www.shucheng.gov.cn/group3/M00/2D/8D/wKgSG2I2smGAH_riAAXwzEuxA3w203.pdf
- 照片：Skylines of Hefei at Tianehu，摄影：钉钉，2019-06-10。
- 照片来源：https://commons.wikimedia.org/wiki/File:Skylines_of_Hefei_at_Tianehu.jpg
- 图片许可：https://creativecommons.org/licenses/by-sa/4.0/

图片采用官方 1280px 缩略图，未修改文件内容；窄屏通过 CSS 裁切显示。使用图片时请保留作者、来源、许可与裁切说明。
