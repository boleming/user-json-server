## json-server一个没有后端代码，但能实现数据增删查改的数据接口

#### 接口示例：（先运行接口才行）
1. 获取所有用户信息
http://localhost:3000/users
2. 获取id为1的用户信息
http://localhost:3000/users/1
3. 获取公司的所有信息
http://localhost:3000/companies
4. 获取单个公司的信息
http://localhost:3000/companies/1
5. 获取所有公司id为3的用户信息
http://localhost:3000/companies/3/users
6. 根据公司名字获取信息
http://localhost:3000/companies?name=Apple
7. 根据多个名字获取公司信息
http://localhost:3000/companies?name=Apple&name=huawei
8. 获取一页中只有两条数据
http://localhost:3000/companies?_page=1&_limit=2
9. 升序排序 asc升序 desc降序
http://localhost:3000/companies?_sort=name&_order=asc
10. 获取年龄30及以上的
http://localhost:3000/users?age_gte=25
11. 获取年龄在25到30之间
http://localhost:3000/users?age_gte=25&age_lte=40
12. 搜索用户信息
http://localhost:3000/users?q=30
#### 具体效果图：
