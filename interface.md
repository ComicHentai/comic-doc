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
	  "errorMsg": "String(可为空)",
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

##### 关于出参部分, 在考虑继续上次阅读部分参数如何接收. 考虑到有用户不登录的情况, 所以还没有写进去


### 搜索页

/search/index

入参

	{
	  "userId": "int(可为空)"
	}

出参

	{
	  "success": "bool(可为空)",
	  "errorMsg": "String(可为空)",
	  "searchHistory": [
	    "String",
	    "..."
	  ]
	}

###搜索结果页

/search/result

入参

	{
	  "comicName": "String"
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

#####搜索结果按照相似度排序

###分类

/classification/index

入参
	
	{
		null
	}

出参

	{
	  "success": "bool(true为空)",
	  "errorMsg": "String",
	  "classification": [
	    {
	      "classifiedId": "int",
	      "classifiedCoverTitle": "String",
	      "classifiedTitle": "String"
	    }
	  ]
	}

###分类详情页

/classification/details

入参

	{
	  "classifiedId": "int",
	  "sortFlag": "String/Other(没想好分类排序该用什么)"
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

###我的

/mine/index

入参

	{
	  "userId": "int(可为空)"
	}

出参

	{
	  "userId": "int",
	  "nickname": "String",
	  "sexy": "String"
	}

###我的收藏

/mine/collection

入参

	{
	  "userId": "int(可为空)"
	}

出参

	{
	  "success": "bool(true为空)",
	  "errorMsg": "String(可为空)",
	  "comic": [
	    {
	      "comicId": "int",
	      "comicTitle": "String",
	      "coverPictureTitle": "String",
	      "updatedTime": "String",
	      "updatedContent": "String",
	      "status": "bool(已完结为true)",
	      "readHistory": "String"
	    },
	    {
	      "...": "..."
	    }
	  ]
	}

###我的专题

/mine/special

入参

	{
	  "userId": "int(可为空)"
	}

出参

	{
	  "success": "bool(true为空)",
	  "errorMsg": "String(可为空)",
	  "special": [
	    {
	      "specialId": "int",
	      "specialTitle": "String",
	      "specialCoverTitle": "String"
	    },
	    {
	      "...": "..."
	    }
	  ]
	}

###专题页

/mine/special/content

入参
	
	{
	  "specialId": "int(可为空)"
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

###历史纪录

/mine/history

入参

	{
	  "userId": "int(可为空)"
	}

出参

	{
	  "success": "bool(true为空)",
	  "errorMsg": "String(可为空)",
	  "comic": [
	    {
	      "comicId": "int",
	      "comicTitle": "String",
	      "coverPictureTitle": "String",
	      "updatedTime": "String",
	      "updatedContent": "String",
	      "status": "bool(已完结为true)",
	      "readHistory": "String"
	    },
	    {
	      "...": "..."
	    }
	  ]
	}