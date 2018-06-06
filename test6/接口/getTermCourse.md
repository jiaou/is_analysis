# 接口：getTermCourse [返回](../Readme.md)
用例： [选课](../用例/选课.md)

- 权限：
    学生/访客：不能使用此接口
    老师：评分

- 功能：
    根据各评分项计算当前实验总分

- API请求地址：
   接口基本地址/v1/api/getTermCourse/<term_id>

- 请求方式 ：
    GET

- 请求参数说明:

     |字段|说明|
     |:-------:|:----------|
     |teacher_id| 教师的工号|
     |student_id| 学生的学号|
     |term_id|学期号|


- 返回实例：

        {
            "status": true,
            "info": null,
            "termCourse":[{
                "coursename":JAVA,
                "course_id":0001,

            }]

        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |coursename|课程名|
  |course_id|课程号|