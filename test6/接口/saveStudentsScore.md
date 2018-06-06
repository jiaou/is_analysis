# 接口：saveStudentsScore [返回](../Readme.md)
用例： [评分](../用例/提交评分.md)

- 权限：
    学生/访客：不能使用此接口
    老师：保存评分

- 功能：
    将该实验各评分项保存在SCORE表内

- API请求地址：
   接口基本地址/v1/api/saveStudentScore

- 请求方式 ：
    GET

    - 请求实例：

            {
                "status": true,
                "info": null,
                "total": 121,

               studenttest[{
                  "sum"：85
                  "STUDENT_ID":0001
                  "TEACHER_ID":0001
                   "studentscore"：[{
                      "score1":15,
                      "score2":25,
                      "score3":20,
                      "score4":25,

                   }]
               }]


            }

- 请求参数说明:

     |参数名称|说明|
     |:-------:|:----------|
     |sum| 总评分|
     |STUDENT_ID|学生的学号|
     |TEST_ID| 实验编号|
     |TEACHER_ID|老师的工号|
     |MEMO|评语|
     |UPDATE_TIME|DATE|评改日期|
     |SCORE1| 评分1,根据学号实验编号保存在SCORE表|
     |SCORE2| 评分2,根据学号实验编号保存在SCORE表|
     |SCORE3| 评分3,根据学号实验编号保存在SCORE表|
     |SCORE4| 评分4,根据学号实验编号保存在SCORE表|

- 返回实例：

        {
            "status": true,
            "info": null,
            "total": 121,

           studenttest[{
              "sum"：85
              "STUDENT_ID":0001
              "TEACHER_ID":0001

           }]


        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |sum|返回总评分|
  |data1|该学生所有实验评分的数组|
  |STUDENT_ID|学号|
  |TEACGER_ID|工号|
