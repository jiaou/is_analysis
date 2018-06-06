# 接口：ShowStu  [返回](../Readme.md)
用例： [学生列表](../用例/学生列表.md)

- 权限：
    学生/访客：不能看到RESULT_SUM，WEB_SUM
    老师：可以看到RESULT_SUM，WEB_SUM。

- 功能：
    返回所有学生的列表。

- API请求地址：
   接口基本地址/v1/api/ShowStu

- 请求方式 ：
    GET

- 请求参数说明:
    无

- 返回实例：

        {
            "status": true,
            "info": null,
            "total": 121,
            "data": [
                {"web_sum": "Y,Y,Y,Y,Y,N",
                "result_sum": "83.75,90,80,80,85,N",
                "githubname": "jiaou",
                "student_id": "201510315203",
                "grade": "软件(本)15-3",
                "name": "林",
                "update_date": "2018-04-02 13:48:01"},
                {
                ...其他学生
                }
            ]
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |total|返回学生人数|
  |data|所有学生的数组|
  |web_sum|网址是否正确的汇总|
  |result_sum|成绩的汇总|
  |githubname|GITHUB 用户名|
  |student_id|学号|
  |grade|班级|
  |name|真实姓名|
  |update_date|GitHUB用户名修改日期|