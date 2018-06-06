# 接口：Login  [返回](../Readme.md)
用例： [登录](../用例/登录.md)

- 功能：
    登录

- 权限：
    未登录用户

- API请求地址：
    接口基本地址/v1/api/Login/

- 请求方式 ：
    POST

- 请求实例：

        {
            "user_id":0001,
            "password"：123213,
        }

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |user_id|用户的user_id值，对应表USERS.USER_ID的值|
  |password|用户的password值，对应表USERS.PASSWORD的值|

- 返回实例：

        {
            "status": true,
            "info": null,
            user[{
            "teacher_id":0001/"student_id":0001，
             "githubname": "jiaou",
            }]
             "name":林榆佳
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |student_id|学号|
  |teacher_id|工号|
  |GITHUB_USERNAME|GITHUB 用户名|
  |GRADE|班级/部门|
  |NAME|真实姓名|
  |UPDATE_DATE|GitHUB用户名修改日期|
