## user接口设计

#### 新增用户
user/signUp

入参

    {
      "userInfo": {
        "username": "String",
        "password": "String",
        "nickname": "String",
        "sexy": "String",
        "email": "String",
        "status": "Integer"
      }
    }

出参

    {
      "isSuccess": "boolean",
      "remark": "String",
      "id": "Integer"
    }

#### 修改用户

user/updated

入参

    {
      "userInfo": {
        "id": "Integer",
        "username": "String",
        "password": "String",
        "nickname": "String",
        "sexy": "String",
        "email": "String",
        "status": "Integer"
      }
    }

出参

    {
      "isSuccess": "boolean",
      "remark": "String",
      "result": "Integer"
    }

#### 删除用户

user/deleted

入参

    {
      "id": "Integer"
    }

出参

	{
      "isSuccess": "boolean",
      "remark": "String",
      "result": "Integer"
    }

#### 批量删除用户

user/deleted/batch

入参

    {
      "idList": [
        "Integer"
      ]
    }

出参

	{
      "isSuccess": "boolean",
      "remark": "String",
      "result": "Integer"
    }

#### 用户验证

user/volatileUser

入参

    {
      "userInfo": {
        "username": "String"
      }
    }

出参

    {
      "isSuccess": "boolean",
      "remark": "String",
      "result": "Integer"
    }



#### 用户登录

user/signIn

入参

    {
      "userInfo": {
        "username": "String",
        "password": "String"
      }
    }

出参

    {
      "isSuccess": "boolean",
      "remark": "String",
      "userInfo": {
        "id": "Integer",
        "username": "String",
        "password": "String",
        "nickname": "String",
        "sexy": "String",
        "email": "String"
      }
    }

























