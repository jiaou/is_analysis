# 接口：setPassword [返回](../Readme.md)
用例： [修改密码](../用例/修改密码.md)

- 权限：
    访客：不能使用此接口
    学生/老师：修改密码

- 功能：
    根据用户ID查询自身密码，然后修改

- API请求地址：
   接口基本地址/v1/api/setPassword

- 请求方式 ：
   POST

- 请求参数说明:

     |字段|说明|
     |:-------:|:----------|
     |student_id|学号|
     |teacher_id|工号|
     |Password|密码|


- 返回实例：

        {
            "status": true,
            "info": 修改成功,
            "Password"：asdwfasdw
            "students_id":0001/"teacher_id":0001

        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |Password|密码|
  |student_id|学号|
  |teacher_id|工号|
