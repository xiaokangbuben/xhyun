# 文章相关接口说明
测试域名：  http://139.199.189.241:8080/liaoliao/

### 1.获取热搜  POST  base/listByType/{type}.do
#### 请求参数
|参数        |必选   |类型    	|说明|
---         |---    |---    	|---
type	    |true  |string       |类型 banner(首页banner位图片)，menu（主页menu）|


#### 响应参数类型说明
|参数        	|类型    	|说明|
|---         	|---    	|---|
|id              |int		|menuId|
|name           |String		|主页menu名称|



#### 响应数据
```
{
  "dataList": [
    {
      "code": 1,
      "validStatus": 1,
      "createTime": 1487257774000,
      "name": "产品中心",
      "id": 31,
      "type": "menu"
    },
    {
      "code": 2,
      "validStatus": 1,
      "createTime": 1487257775000,
      "name": "解决方案",
      "id": 32,
      "type": "menu"
    },
    {
      "code": 3,
      "validStatus": 1,
      "createTime": 1487257776000,
      "name": "服务项目",
      "id": 33,
      "type": "menu"
    },
    {
      "code": 4,
      "validStatus": 1,
      "createTime": 1487257777000,
      "name": "新闻中心",
      "id": 34,
      "type": "menu"
    },
    {
      "code": 5,
      "validStatus": 1,
      "createTime": 1487257778000,
      "name": "联系我们",
      "id": 35,
      "type": "menu"
    },
    {
      "code": 6,
      "validStatus": 1,
      "createTime": 1487257779000,
      "name": "关于我们",
      "id": 36,
      "type": "menu"
    }
  ],
  "status": "success"
}
```