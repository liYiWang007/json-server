# json-server
test restful api/ postman
//获取所有用户信息  
http://localhost:3000/

//获取id为1的用户信息  
http://localhost:3000/user/1

//获取公司的所有信息  
http://localhost:3000/companies

//获取单个公司信息（如1）
http://localhost:3000/companies/1

//获取id为1的公司的所有用户信息
http://localhost:3000/companies/1/user

//获取wawa公司
http://localhost:3000/companies?name=wawa

//根据多个公司名字获取信息（?name&name=）
http://localhost:3000/companies?name=wawa&name=suckerpunch

//一页内（_page=1）只显示两条数据（_limit=2）
http://localhost:3000/uers?_page=1&_limit=2

//按name为标准（_sort）进行排序
//升序规则（asc）
//降序规则（desc）
http://localhost:3000/uers?_sort=name&_order=asc

//筛选年龄为30或以上的用户
//_gte 大于
//_lte 小于
//age_gte=10&age_lte=20 在10~20以内  
http://localhost:3000/uers?age_gte=30

//筛选名字包含e的用户 q= 过滤
http://localhost:3000/uers?q=e
