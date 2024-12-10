## POST https://mycompagny.com/api/v1/students
~~~json
{
    "firstName":"Yousssou",
    "lastName":"Cisse",
    "createdBy": "<UUID>"

}
~~~

## POST https://mycompagny.com/api/v1/enrollements

~~~json
{
    "idStudent":"<UUID>",
    "idCourse":"<UUID>",
    "createdBy": "<UUID>"

}
~~~

## POST https://mycompagny.com/api/v1/courses
~~~json
{
  "name":"JAVA",
  "createdBy": "<UUID>"
}
~~~
## GET https://mycompagny.com/api/v1/students/1
~~~json
{
  "body":{
    "id":"<UUID>",
    "firstName":"Yousssou",
    "lastName":"Cisse",
    "metaData":{
      "status": "ACTIVATE",
      "version": 1,
      "createdBy": "<UUID>",
      "createdAt": "timeStamp",
      "updatedBy": "<UUID>"
    }
  },
  "code": 201,
  "msg": "SUCCESS"
}
~~~
## GET https://mycompagny.com/api/v1/students
~~~json
{
  "body":[
    {
      "id":"<UUID>",
      "firstName":"Yousssou",
      "lastName":"Cisse",
      "metaData":{
        "status": "ACTIVATE",
        "version": 1,
        "createdBy": "<UUID>",
        "createdAt": "timeStamp",
        "updatedBy": "<UUID>"
      }
    },
    {
      "id":"<UUID>",
      "firstName":"Laye",
      "lastName":"Ba",
      "metaData":{
        "status": "ACTIVATE",
        "version": 1,
        "createdBy": "<UUID>",
        "createdAt": "timeStamp",
        "updatedBy": "<UUID>"
      }
    }
  ],
  "code": 201,
  "msg": "SUCCESS"
}
~~~
## GET https://mycompagny.com/api/v1/enrollements/students?idCourse=1

~~~json
{
  "body": {
    "idCourse":1,
    "students": [
      {
        "id": "<UUID>",
        "firstName": "Yousssou",
        "lastName": "Cisse",
        "metaData": {
          "status": "ACTIVATE",
          "version": 1,
          "createdBy": "<UUID>",
          "createdAt": "timeStamp",
          "updatedBy": "<UUID>"
        }
      },
      {
        "id": "<UUID>",
        "firstName": "Laye",
        "lastName": "Ba",
        "metaData": {
          "status": "ACTIVATE",
          "version": 1,
          "createdBy": "<UUID>",
          "createdAt": "timeStamp",
          "updatedBy": "<UUID>"
        }
      }
    ]
  },
  "code": 201,
  "msg": "SUCCESS"
}
~~~

