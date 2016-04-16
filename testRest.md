### ComicController

#### comic/add/info

localhost:8080/comic/add/info?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","comicDto":{"title":"title","coverTitle":"coverTitle","author":"author","introduction":"introduction","contentTitle":"contentTitle"}}

入参

    {
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "comic": {
          "title": "String",
          "coverTitle": "String",
          "author": "String",
          "introduction": "String",
          "contentTitle": "String"
        }
      }
    }


出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### comic/deleted

localhost:8080/comic/deleted?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","comicDtos":[{"id":7},{"id":8}]}

入参

    {
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "comics": [
            {
              "id": "Integer"
            }
        ]
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### comic/updated

localhost:8080/comic/updated?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","comicDto":{"id":7,"title":"title01","coverTitle":"coverTitle","author":"author","introduction":"introduction","contentTitle":"contentTitle"}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "comic": {
          "id": "Integer",
          "title": "String",
          "coverTitle": "String",
          "author": "String",
          "introduction": "String",
          "contentTitle": "String"
        }
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### comic/index

localhost:8080/comic/index?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","comicDto":{"id":1}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "comic": {
          "id": "Integer"
        }
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": {
          "pageSize": Integer,
          "startRecord": null,
          "id": null,
          "created": null,
          "createdBefore": null,
          "createdAfter": null,
          "updated": null,
          "updatedBefore": null,
          "updatedAfter": null,
          "status": null,
          "isDeleted": null,
          "classifiedId": null,
          "targetId": null,
          "targetType": null,
          "comicByClassfied": {},
          "specialByClassfied": {},
          "comic": {
            "com.comichentai.dto.ComicDto@bd1e9ad5": [
              {
                "pageSize": Integer,
                "startRecord": null,
                "id": Integer,
                "created": Integer,
                "createdBefore": null,
                "createdAfter": null,
                "updated": Integer,
                "updatedBefore": null,
                "updatedAfter": null,
                "status": 0,
                "isDeleted": "String",
                "title": "String",
                "coverTitle": "String",
                "currentPage": null
              }
            ]
          },
          "special": {},
          "currentPage": null
        },
        "pageMap": "String",
        "isEnd": boolean
      }
    }

#### comic/getComic

 //这个和welcome/index一样一样一样的！！

### UserInfoController

#### user/index

localhost:8080/user/index?_mode=debug&_auth=debug&data={"token":{"userInfoId":1},"deviceId":"deviceId"}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": {
          "pageSize": Integer,
          "startRecord": null,
          "id": Integer,
          "created": Integer,
          "createdBefore": null,
          "createdAfter": null,
          "updated": Integer,
          "updatedBefore": null,
          "updatedAfter": null,
          "status": Integer,
          "isDeleted": "String",
          "coverTitle": null,
          "username": "String",
          "password": "String",
          "nickname": "String",
          "sexy": "String",
          "email": "String",
          "currentPage": null
        }
      }
    }

#### user/signUp

localhost:8080/user/signUp?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","userInfo":{"coverTitle":"coverTitle","username":"username","password":"password","nickname":"nickname","sexy":"sexy","email":"email"}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
        "userInfo":{
        	"coverTitle": "String",
            "username": "String",
            "password": "String",
            "nickname": "String",
            "sexy": "String",
            "email": "String"
        }
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### user/updated

localhost:8080/user/updated?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","userInfo":{"id":1,"coverTitle":"coverTitle","username":"username01","password":"password","nickname":"nickname","sexy":"sexy","email":"email"}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
        "userInfo":{
        	"id": "Integer",
        	"coverTitle": "String",
            "username": "String",
            "password": "String",
            "nickname": "String",
            "sexy": "String",
            "email": "String"
        }
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

### user/deleted

localhost:8080/user/deleted?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","userInfo":{"id":2}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
        "userInfo":{
        	"id": "Integer"
        }
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### user/deleted/batch

localhost:8080/user/deleted/batch?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","userInfos":[{"id":2},{"id":1}]}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
        "userInfos":[
        	{
        		"id": "Integer"
        	}
        ]
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### user/signIn

localhost:8080/user/signIn?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","userInfo":{"username":"username", "password":"password"}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
        "userInfo":{
            "username": "String",
            "password": "String"
        }
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": "String" -> token
      }
    }

#### user/volatile

localhost:8080/user/volatile?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","userInfo":{"nickname":"haha"}}

localhost:8080/user/volatile?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","userInfo":{"username":"haha"}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
        "userInfo":{
            "username/nickname": "String"
        }
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }


### WelcomeController

#### welcome/index

localhost:8080/welcome/index?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId"}

入参

    {
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
      }
    }

出参

    {
      "success": "boolean",
      "returnMsg": "String",
      "data": {
        "data": [
          {
            "pageSize": "Integer",
            "startRecord": null,
            "id": "Integer",
            "created": "Integer",
            "createdBefore": null,
            "createdAfter": null,
            "updated": "Integer",
            "updatedBefore": null,
            "updatedAfter": null,
            "status": "Integer",
            "isDeleted": "String",
            "title": "String",
            "coverTitle": "String",
            "author": "String",
            "introduction": "String",
            "contentTitle": "String",
            "currentPage": null
          }
        ],
        "pageMap": "String",
        "isEnd": "boolean"
      }
    }

### ClassifiedContrller

#### classification/category/add

localhost:8080/classification/category/add?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","category":{"classifiedId":1,"targetId":1,"targetType":1}}

入参

    {
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "category": {
          "classifiedId": "Integer",
          "targetId": "Integer",
          "targetType": "Integer"
        }
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### classification/category/deleted

localhost:8080/classification/category/deleted?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","categorys":[{"id":1},{"id":2}]}

入参

    {
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "categorys": [
          {
            "id": "Integer"
          }
        ]
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### classification/add

localhost:8080/classification/add?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","classified":{"title":"title","coverTitle":"coverTitle"}}

入参

    {
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "classified": {
          "title": "String",
          "coverTitle": "String"
        }
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### classification/deleted

localhost:8080/classification/deleted?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","classified":{"id":"1"}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "classified": {
          "id": "Integer"
        }
      }
    }

出参

        {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### classification/deleted/batch

localhost:8080/classification/deleted/batch?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","classifieds":[{"id":1},{"id":2}]}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "classifieds": [
          {
            "id": "Integer"
          }
        ]
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### classification/updated

localhost:8080/classification/updated?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","classified":{"id":1,"title":"[修改测试后名称01]","coverTitle":"[修改测试后封面01]"}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "classified": {
          "id": "Integer",
          "title": "String",
          "coverTitle": "String"
        }
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### classification/index

localhost:8080/classification/index?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId"}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": [
          {
            "pageSize": Integer,
            "startRecord": null,
            "id": Integer,
            "created": Integer,
            "createdBefore": null,
            "createdAfter": null,
            "updated": Integer,
            "updatedBefore": null,
            "updatedAfter": null,
            "status": Integer,
            "isDeleted": String,
            "title": "String",
            "coverTitle": "String",
            "currentPage": null
          }
        ],
        "pageMap": "String",
        "isEnd": boolean
      }
    }

#### classification/comic/detail

localhost:8080/classification/comic/detail?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","classified":{"id":1}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
        "classified":{
        	"id": "Integer"
        }
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "date": {
          "pageSize": Integer,
          "startRecord": null,
          "id": null,
          "created": null,
          "createdBefore": null,
          "createdAfter": null,
          "updated": null,
          "updatedBefore": null,
          "updatedAfter": null,
          "status": null,
          "isDeleted": null,
          "classifiedId": null,
          "targetId": null,
          "targetType": null,
          "comicByClassfied": {
            "com.comichentai.dto.ClassifiedDto@5cf830cc": [
              {
                "pageSize": Integer,
                "startRecord": null,
                "id": Integer,
                "created": Integer,
                "createdBefore": null,
                "createdAfter": null,
                "updated": Integer,
                "updatedBefore": null,
                "updatedAfter": null,
                "status": 0,
                "isDeleted": "String",
                "title": "String",
                "coverTitle": "String",
                "author": "String",
                "introduction": "String",
                "contentTitle": "String",
                "currentPage": null
              }
            ]
          },
          "specialByClassfied": {},
          "comic": {},
          "special": {},
          "currentPage": null
        },
        "pageMap": "String",
        "isEnd": boolean
      }
    }

#### classification/special/detail

	//TODO

#### classification/volatile

localhost:8080/classification/volatile?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","classified":{"title": "test02"}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String"
        "classified":{
        	"title": "String"
        }
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

### SpecialController

#### special/add/info

localhost:8080/special/addInfo?_mode=debug&_auth=debug&data={"token":{"userInfoId":1},"deviceId":"deviceId","specialTitle":"specialTitle01"}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
      	"token"："String",
        "deviceId":"String",
        "specialTitle": "String"
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### special/deleted

localhost:8080/special/deleted?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","specials":[{"id":1}]}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "specials": [
          {
            "id": "Integer"
          }
        ]
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### special/add/comic

localhost:8080/special/add/comic?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","special":{"id":1},"comic":{"id":1}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "special":{
           "id": "Integer"
        }
        "comic": {
        	"id": "Integer"
        }
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### special/deleted/comic

localhost:8080/special/deleted/comic?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","special":{"id":1},"comic":{"id":1}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "special":{
           "id": "Integer"
        }
        "comic": {
        	"id": "Integer"
        }
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### special/content

localhost:8080/special/content?_mode=debug&_auth=debug&data={"token":"token","deviceId":"deviceId","special":{"id":1}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "special":{
           "id": "Integer"
        }
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": {
          "pageSize": Integer,
          "startRecord": null,
          "id": null,
          "created": null,
          "createdBefore": null,
          "createdAfter": null,
          "updated": null,
          "updatedBefore": null,
          "updatedAfter": null,
          "status": null,
          "isDeleted": null,
          "specialId": null,
          "comicId": null,
          "jump": {
            "com.comichentai.dto.SpecialDto@cd407d60": [
              {
                "pageSize": Integer,
                "startRecord": null,
                "id": Integer,
                "created": Integer,
                "createdBefore": null,
                "createdAfter": null,
                "updated": Integer,
                "updatedBefore": null,
                "updatedAfter": null,
                "status": 0,
                "isDeleted": "String",
                "title": "String",
                "coverTitle": "String",
                "author": "String",
                "introduction": "String",
                "contentTitle": "String",
                "currentPage": null
              }
            ]
          },
          "currentPage": null
        },
        "pageMap": "String",
        "isEnd": boolean
      }
    }

### MineController

#### mine/collection/add

localhost:8080/mine/collection/add?_mode=debug&_auth=debug&data={"token":{"userInfoId":1},"deviceId":"deviceId","comic":{"id":1}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "comic": {
        	"id": "Integer"
        }
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### mine/collection/deleted

localhost:8080/mine/collection/deleted?_mode=debug&_auth=debug&data={"token":{"userInfoId":1},"deviceId":"deviceId","comic":{"id":3}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "comic": {
        	"id": "Integer"
        }
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### mine/collection/index

localhost:8080/mine/collection/index?_mode=debug&_auth=debug&data={"token":{"userInfoId":1},"deviceId":"deviceId"}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String"
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": {
          "pageSize": Integer,
          "startRecord": null,
          "id": null,
          "created": null,
          "createdBefore": null,
          "createdAfter": null,
          "updated": null,
          "updatedBefore": null,
          "updatedAfter": null,
          "status": null,
          "isDeleted": null,
          "userId": null,
          "targetId": null,
          "targetType": null,
          "favoriteComic": {
            "com.comichentai.dto.UserInfoDto@31bd6b8c": [
              {
                "pageSize": Integer,
                "startRecord": null,
                "id": Integer,
                "created": Integer,
                "createdBefore": null,
                "createdAfter": null,
                "updated": 1457859124,
                "updatedBefore": null,
                "updatedAfter": null,
                "status": 0,
                "isDeleted": "String",
                "title": "String",
                "coverTitle": "String",
                "author": "String",
                "introduction": "String",
                "contentTitle": "String",
                "currentPage": null
              }
            ]
          },
          "favoriteSpecial": {},
          "currentPage": null
        },
        "pageMap": "String",
        "isEnd": boolean
      }
    }

#### mine/special/add

localhost:8080/mine/special/add?_mode=debug&_auth=debug&data={"token":{"userInfoId":1},"deviceId":"deviceId","special":{"id":1}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "special": {
        	"id": "Integer"
        }
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### mine/special/deleted

localhost:8080/mine/special/deleted?_mode=debug&_auth=debug&data={"token":{"userInfoId":1},"deviceId":"deviceId","special":{"id":1}}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String",
        "special": {
        	"id": "Integer"
        }
      }
    }

出参

	{
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": Integer
      }
    }

#### mine/special/index

localhost:8080/mine/special/index?_mode=debug&_auth=debug&data={"token":{"userInfoId":1},"deviceId":"deviceId"}

入参

	{
      "_mode": "debug",
      "_auth": "debug",
      "data": {
        "token": "String",
        "deviceId": "String"
      }
    }

出参

    {
      "success": boolean,
      "returnMsg": "String",
      "data": {
        "data": {
          "pageSize": Integer,
          "startRecord": null,
          "id": null,
          "created": null,
          "createdBefore": null,
          "createdAfter": null,
          "updated": null,
          "updatedBefore": null,
          "updatedAfter": null,
          "status": null,
          "isDeleted": null,
          "userId": null,
          "targetId": null,
          "targetType": null,
          "favoriteComic": {},
          "favoriteSpecial": {
            "com.comichentai.dto.UserInfoDto@4ebb7473": [
              {
                "pageSize": Integer,
                "startRecord": null,
                "id": Integer,
                "created": Integer,
                "createdBefore": null,
                "createdAfter": null,
                "updated": Integer,
                "updatedBefore": null,
                "updatedAfter": null,
                "status": Integer,
                "isDeleted": "String",
                "title": "String",
                "userId": Integer,
                "currentPage": null
              }
            ]
          },
          "currentPage": null
        },
        "pageMap": "String",
        "isEnd": boolean
      }
    }