### 首页

/welcome/index

入参

	{
		"userId":"int(可为空)"
	}

出参

	{
	  "success": "bool(true为空)",
	  "errorMsg": "String(可为空)",
	  "comic": [
	    {
	      "comicId": "int",
	      "comicTitle": "String",
	      "author": "String",
	      "coverPictureTitle": "String",
	      "introduction": "String",
		  "updatedContent": "String",
	      "status": "bool(已完结为true)"
	    },
	    {
	      "...": "..."
	    }
	  ]
	}

### 漫画详情页

/comic/index

入参

	{
	  "comicId": "int",
	  "userId": "int(可为空)"
	}

出参

	{
	  "success": "bool(true为空)",
	  "errorMsg": "String",
	  "comic": {
	    "comicTitle": "String",
	    "coverPictureTitle": "String",
	    "author": "String",
		"status": "bool(已完结为true)",
	    "updatedTime": "String",
	    "updatedContent": "String",
	    "introduction": "String",
	    "contentTitle": "String"
	  }
	}

