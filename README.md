## json-server一个没有后端代码，但能实现数据增删查改的数据接口
#### 前端代码：
> https://github.com/boleming/user-management
#### 如何安装并运行：
1. 全局安装：
```
npm install -g json-server
```
2. 切换盘符：
```
cd F:(具体路径）

F:
```
3. 安装json-server：(所有属性选择均回即可)
```
npm init
```
4. 初始化json-server：
```
npm install json-server --save
```
5. 配置package.json:
```
"scripts": {
  "json:server": "json-server --watch mv.json"
}
```
6.运行代码：
```
npm run json:server
```
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
![image](https://raw.githubusercontent.com/boleming/user-json-server/master/imgs/data1.png)
![image](https://raw.githubusercontent.com/boleming/user-json-server/master/imgs/data2.png)
