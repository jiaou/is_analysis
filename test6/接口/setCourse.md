# 接口：getCourse [返回](../Readme.md)
用例： [评分](../用例/评定成绩.md)

- 权限：
    访客：不能使用此接口
    学生/老师：选择课程

- 功能：
    根据工号/学号选择有关课程，老师先选，学生后选

- API请求地址：
   接口基本地址/v1/api/getCourse

- 请求方式 ：
    POST

- 请求参数说明:

     |字段|说明|
     |:-------:|:----------|
     |student_id|学号|
     |teacher_id|工号|
     |course_id|课程号|


- 返回实例：

        {
            "status": true,
            "info": 选课成功,
             course[{
                "coursename":java，
                "course_id":0001
             }]
            "students_id":0001/"teacher_id":0001

        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |coursename|课程名称|
  |course_id|课程号|
  |student_id|学号|
  |teacher_id|工号|
