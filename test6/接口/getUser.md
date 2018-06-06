# 接口：setUser [返回](../Readme.md)
用例： [修改用户信息](../用例/修改用户信息.md)

- 权限：
    访客：不能使用此接口
    学生/老师：查询用户信息

- 功能：
    根据用户ID查询自身信息，然后修改，老师可以查询学生

- API请求地址：
   接口基本地址/v1/api/getUser/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:

     |字段|说明|
     |:-------:|:----------|
     |user_id|用户ID|
     |GITHUB_USERNAME|GITHUB 用户名|
     |STUDENT_ID|学号|
     |GRADE|班级|
     |NAME|真实姓名|
     |UPDATE_DATE|GitHUB用户名修改日期|


- 返回实例：

        {
            "status": true,
            "info": 修改成功,

            "students_id":0001/"teacher_id":0001
             userdata[{
                           "GITHUBNAME": "jiaou1",
                             "STUDENT_ID": "201510315505",
                             "GRADE": "软件(本)15-3",
                             "NAME": "林",
                             "UPDATE_DATE": "2018-04-02 13:48:02"},
             }]

        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |Password|密码|
  |student_id|学号|
  |teacher_id|工号|
  |GITHUB_USERNAME|GITHUB 用户名|
  |USER_ID|用户ID|
  |GRADE|班级(学生才有）|
  |NAME|真实姓名|
  |UPDATE_DATE|GitHUB用户名修改日期|