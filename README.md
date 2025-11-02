# 计算机实验室排课与查询系统

## 前言

本项目是基于SSM框架（Spring、SpringMVC、MyBatis）的计算机实验室排课与查询系统，结合前端技术如JavaScript、Vue.js、CSS3和Uniapp，以及微信小程序，旨在为高校计算机实验室提供一个便捷、高效的课程安排与查询解决方案。

## 内容介绍

系统主要包括以下几个模块：实验室管理、课程管理、排课管理、查询管理以及微信小程序端。实验室管理模块负责实验室信息的增删改查；课程管理模块负责课程信息的维护；排课管理模块根据实验室和课程信息进行排课；查询管理模块方便师生查询课程安排；微信小程序端则提供移动端访问功能。

## 技术介绍

- 语言：Java
- 使用框架：Spring、SpringMVC、MyBatis，微信小程序
- 前端技术：JS、Vue、CSS3，Uniapp
- 开发工具：IDEA/Eclipse，Uniapp
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven: apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

## 核心代码

以下是项目中的一个核心代码片段，展示了如何使用MyBatis进行课程查询：

```java
// CourseMapper.xml
<mapper namespace="com.lab.schedule.mapper.CourseMapper">
    <select id="selectCourseList" resultType="com.lab.schedule.entity.Course">
        SELECT * FROM course
        <where>
            <if test="courseName != null and courseName != ''">
                AND course_name LIKE CONCAT('%', #{courseName}, '%')
            </if>
        </where>
    </select>
</mapper>
```

```java
// CourseMapper.java
public interface CourseMapper {
    List<Course> selectCourseList(@Param("courseName") String courseName);
}
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

## 项目截图
![封面图片](https://img12.360buyimg.com/ddimg/jfs/t1/331219/29/12762/84846/68c4de64F70622b1b/cdceb67ae7985548.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/332724/35/12739/31127/68c4de3cFdbda3b38/fa22488b00268a0f.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/336187/24/10097/34978/68c4de3cFf3216068/8d36df3961abc950.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/346028/15/2658/28174/68c4de3cF52cd35ba/aabdff53da6abcb3.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/332030/29/12600/21451/68c4de3dF7d90990c/d519b5144de94dee.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/329043/32/12898/32629/68c4de3dFf565eb7e/2829e873e5ba869f.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/328648/1/19691/54870/68c4de3dF3dc54f1d/fa4bc42ffe8faea0.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/336480/22/10159/12542/68c4de3dF31c8529c/5a7beab68459fa9d.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/350699/37/2859/9026/68c4de3dF89f1629f/f7e00ffe84fde6ba.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/343249/1/2799/23771/68c4de3dF4bf92ce9/8052d99ecf170ea9.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
