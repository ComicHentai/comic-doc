### ��ҳ

/welcome/index

���

	{
		"userId":"int(��Ϊ��)"
	}

����

	{
	  "success": "bool(trueΪ��)",
	  "errorMsg": "String(��Ϊ��)",
	  "comic": [
	    {
	      "comicId": "int",
	      "comicTitle": "String",
	      "author": "String",
	      "coverPictureTitle": "String",
	      "introduction": "String",
		  "updatedContent": "String",
	      "status": "bool(�����Ϊtrue)"
	    },
	    {
	      "...": "..."
	    }
	  ]
	}

### ��������ҳ

/comic/index

���

	{
	  "comicId": "int",
	  "userId": "int(��Ϊ��)"
	}

����

	{
	  "success": "bool(trueΪ��)",
	  "errorMsg": "String",
	  "comic": {
	    "comicTitle": "String",
	    "coverPictureTitle": "String",
	    "author": "String",
		"status": "bool(�����Ϊtrue)",
	    "updatedTime": "String",
	    "updatedContent": "String",
	    "introduction": "String",
	    "contentTitle": "String"
	  }
	}

