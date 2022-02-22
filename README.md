# douyin
#### 抖音数据采集，原生官方api 支持日采百万
#### 抖音打印机 直播打印机 抖音直播 抖音弹幕 直播弹幕
## 用户搜索
```
/dy/search/user
``` 
### 参数:
- username 搜索关键词
- pageIndex 翻页参数，根据结果返回的cursor传入作为下一页翻页参数，初始为0

## 视频搜索 
```
/dy/search/v"
```
### 参数:
- vname 搜索关键词
- pageIndex 翻页参数，根据结果返回的cursor传入作为下一页翻页参数，**初始为0**
- soutType 筛选类型：综合=0，最多点赞=1，最新=2
- timeRange 时间筛选：不限=0，一天=1，一周=7，半年=180

## 话题搜索
```
/dy/search/topic
```
### 参数:
- topic 搜索关键词
- pageIndex 翻页参数，根据结果返回的cursor传入作为下一页翻页参数，**初始为0**

## 用户信息（uid查询）
```
/dy/user/info/uid
```
### 参数:
- uid 

## 用户信息（sec_id查询）
```
/dy/user/info/secid
```
### 参数:
- secId 用户sec_id，分享链接即可看见

## 用户信息（抖音号）
```
/dy/user/info/dyid
```
### 参数:
- dyId 抖音号

## 用户作品列表
```
/dy/user/videos
```
### 参数:
- uid 用户uid，非抖音号
- pageIndex 翻页游标，根据结果返回的max_cursor传入作为下一页翻页参数，初始为0

## 用户喜欢列表
```
/dy/user/likes
```
### 参数:
- uid 用户uid，非抖音号
- pageIndex 翻页游标，根据结果返回的max_cursor传入作为下一页翻页参数，初始为0

## 用户关注列表
```
/dy/user/focus
```
### 参数:
- uid 用户uid，非抖音号
- pageIndex 翻页游标，根据结果返回的min_time传入作为下一页翻页参数，**初始为0**

## 用户粉丝列表
```
/dy/user/fans
```
### 参数:
- uid 用户uid，非抖音号
- pageIndex 翻页游标，根据结果返回的min_time传入作为下一页翻页参数，**初始为0**

## 用户橱窗
```
/dy/user/sales
```
### 参数:
- uid 用户uid，非抖音号

## 抖音商品详情
```
/dy/user/goods/detail
```
### 参数:
- goodsId 商品id

## 抖音视频详情
```
/dy/v/detail
```
### 参数:
- vid 视频id

## 抖音视频评论列表
```
/dy/v/comments
```
### 参数:
- vid 视频id
- pageIndex 翻页游标，根据结果返回的cursor传入作为下一页翻页参数，**初始为0**

## 抖音视频无水印解析
```
/dy/v/noicon
```
### 参数:
- vid 视频id

## 直播弹幕获取
## 其他

```
有任何问题可交流学习  
请勿使用本服务于商用   
请勿使用本服务大量抓取   
若因使用本服务与平台造成不必要的纠纷，本人盖不负责  
本人纯粹技术爱好，若侵犯贵公司的权益，请告知  
```

有需要的[联系QQ45497494](https://qr.api.cli.im/newqr/create?data=https%253A%252F%252Fqm.qq.com%252Fcgi-bin%252Fqm%252Fqr%253Fk%253DgsXU_14bQsI8BdSevrFzHU7vIYnRCnFQ%2526noverify%253D0&level=H&transparent=false&bgcolor=%23FFFFFF&forecolor=%23000000&blockpixel=12&marginblock=1&logourl=&logoshape=no&size=500&kid=cliim&key=211db538a2ba8c28441f5d952fe165db)

### 另有[小红书](https://github.com/canglingzhiyue/xiaohongshu)数据采集
