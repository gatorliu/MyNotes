Code Review
=============================
> Everythings about codereview

## Database
> Something about database
* 需要整合不同的設定到 Data Dictionary


## Major Problem
1. 後台 Timeout機制是否合宜?



## 已修改問題:

### 共通性問題
#### 前台
#### 後台
> also see svn log
1. `Controllers/NewsController.cs` :  performance issue
	``` C#
	# bad
	int pageSize = new baseController().getConfigPageSize();	
	# good 
	int pageSize = this.getConfigPageSize();
	
	# because `public class NewsController : baseController`
	# so we don't need to create a new object `baseController`
	```

2. menubar click 隱藏後無法再出現: `Scripts\jqueryslidemenu2.js`
	``` JavaScript
	// line. 46
	hide() -> toggle()
	```

#### BOTH




## 未修改問題:

### 聯絡我們
#### 前台
1. 問題內容分行，輸出HTML時未轉換成 <br>

#### 後台
1. 問題內容分行，輸出HTML時未轉換成 <br>
1. 無`處理狀態`的搜尋
1. 回復者id，是否需要自動帶入?
1. 新增無成功訊息 
1. 刪除問題?  是否可以刪除? 只有後臺的可以刪除？真刪?
1. 欄位檢查
1. 會員編號的必要性?

### 上傳


### 課程 : 商品管理 : 產品管理 
#### 前台
#### 後台
1. 列表缺 修改日(DB也沒有修改日 修改人 )
1. 產品編號未檢查是否重複(自動建立?)
1. DB缺銷售對象欄位

#### BOTH


### 


none




