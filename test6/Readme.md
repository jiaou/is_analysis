# 基于GitHub的实验管理平台的分析与设计

### 成都大学信息科学与工程学院

<table >
<tr>
<td align="center">学号</td>
<td align="center">班级</td>
<td align="center">姓名</td>
<td align="center">照片</td>
</tr>
<tr>
<td>201510414309</td>
<td>15级软件三班</td>
<td>林榆佳</td>
<td><img src="1.png" width="50" /></td>
</tr>
</table>

## 1. 概述
- 基于GitHub的实验管理平台的作用是在线管理实验成绩的Web应用系统。学生和老师的实验内容均存放在GitHUB
页面上。
- 学生的功能主要有：一是设置自己的GitHub用户名，二是查询自己的实验成绩。学生的GitHub用户名是公开的，但成绩不公开。
- 老师的功能主要有：一是批改每个学生的成绩，二是查看每个学生的成绩。
- 老师和学生都能通过本系统的链接方便地跳转到学生的每个GitHUB实验目录，以便批改实验或者查看实验情况。
- 实验成绩按数字分数计算，每项实验的满分为100分，最低为0分。
- 系统自动计算每个学生的所有实验的平均分。
- 选课
- 多个课程多个实验评定
- 不同课程不同学生

## 2. 系统总体结构
![](系统总体结构.png)

界面设计参见：https://jiaou.github/is_analysis/test6/ui/index.html

## 3. 用例图设计 [源码](src/Usecase.puml)
![](Usecase.png)

## 4. 类图设计 [源码](src/class.puml)
![](类图.png)

## 5. 数据库设计
- ### [参见数据库设计](数据库设计.md)

## 6. 用例及界面详细设计
- ### [“学生列表”用例](./用例/学生列表.md),[界面](https://jiaou.github.io/is_analysis/test6/ui/index.html)
- ### [“评定成绩”用例](./用例/评定成绩.md),[界面](https://jiaou.github.io/is_analysis/test6/ui/评定成绩.html)
- ### [“查看成绩”用例](./用例/查看成绩.md),[界面](https://jiaou.github.io/is_analysis/test6/ui/查看成绩.html)
- ### [“修改密码”用例](./用例/修改密码.md),[界面](https://jiaou.github.io/is_analysis/test6/ui/顶部菜单.html)
- ### [“修改用户信息”用例](./用例/修改用户信息.md),[界面](https://jiaou.github.io/is_analysis/test6/ui/顶部菜单.html)
- ### [“查看用户信息”用例](./用例/查看用户信息.md),[界面](https://jiaou.github.io/is_analysis/test6/ui/顶部菜单.html)
- ### [“选课”用例](./用例/选课.md),[界面](https://jiaou.github.io/is_analysis/test6/ui/选择课程.html)
- ### [“登出”用例](./用例/登出.md),[界面](https://jiaou.github.io/is_analysis/test6/ui/顶部菜单.html)
- ### [“登录”用例](./用例/登录.md),[界面](https://jiaou.github.io/is_analysis/test6/ui/登录.html)
