
### 请求地址

/api/c/compapi/v2/cc/delete_user_group/



### 请求方法

POST


### 功能描述

删除用户分组

### 请求参数


#### 通用参数

| 字段 | 类型 | 必选 |  描述 |
|-----------|------------|--------|------------|
| bk_app_code  |  string    | 是 | 应用ID     |
| bk_app_secret|  string    | 是 | 安全密钥(应用 TOKEN)，可以通过 蓝鲸智云开发者中心 -&gt; 点击应用ID -&gt; 基本信息 获取 |
| bk_token     |  string    | 否 | 当前用户登录态，bk_token与bk_username必须一个有效，bk_token可以通过Cookie获取 |
| bk_username  |  string    | 否 | 当前用户用户名，应用免登录态验证白名单中的应用，用此字段指定当前用户 |

#### 接口参数

| 字段                |  类型       | 必选   |  描述       |
|---------------------|-------------|--------|-------------|
| bk_supplier_account | string      | 是     | 开发商账号  |
| group_id            | string      | 是     | 分组ID      |


### 请求参数示例

```python

{
    "bk_supplier_account": "0",
    "delete":{
        "group_id": "test"    
    }
}
```


### 返回结果示例

```python

{
    "result": true,
    "code": 0,
    "message": "",
    "data":""
}
```