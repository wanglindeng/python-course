# python-course

##9.26日课后实践##
>>
1.tuple=('abcd',786,2.23,'runoob',70.2)
print(tuple)
('abcd', 786, 2.23, 'runoob', 70.2)

2.print(tuple[0:3])
 ('abcd', 786, 2.23)

3.print(tuple[1:-1])
  (786, 2.23, 'runoob')

4.print(tuple*2)
 	('abcd', 786, 2.23, 'runoob', 70.2, 'abcd', 786, 2.23, 'runoob', 70.2)

5.tuplelist=(123,'tunoob')
print(tuplelist)
(123, 'tunoob')

6.print(tuple+tuplelist)
  ('abcd', 786, 2.23, 'runoob', 70.2, 123, 'tunoob')

7. tup = (1, 2, 3, 4, 5, 6)
#tup[0]=11  #不能赋值，报错
tupl = (['a',16,'0'], 2, 3, 4, 5, 6)
tupl[0][1]='OH'
print (tupl)
(['a', 'OH', '0'], 2, 3, 4, 5, 6)

8.d={'name':'zara','age':7,'class':'first'}
print(d['name'])
zara

9.d['gender']='female'
print(d)
{'name': 'zara', 'age': 7, 'class': 'first', 'gender': 'female'}

10.d['age']=8
d['school']='high school'
print(d)
{'name': 'zara', 'age': 8, 'class': 'first', 'gender': 'female', 'school': 'high school'}

11.d.update({'age':10,'school':'college'})
print(d)
{'name': 'zara', 'age': 10, 'class': 'first', 'gender': 'female', 'school': 'college'}

12.del d['gender']
print(d)
{'name': 'zara', 'age': 10, 'class': 'first', 'school': 'college'}

13.d.clear()
print(d)
{}

14.var = {'zhangwang','zhangbo','zhanglang'}
print(var,type(var))
{'zhanglang', 'zhangwang', 'zhangbo'} <class 'set'>

15.result = 'zhangwang'in var
print(result)
True

16.var.add('zhangfei')
print(var)
{'zhangbo', 'zahngfei', 'zhangfei', 'zhanglang', 'zhangwang'}

17.var.update('zhangfei')
print(var)
{'h', 'a', 'n', 'e', 'i', 'g', 'z', 'zhangbo', 'zahngfei', 'f', 'zhangfei', 'zhanglang', 'zhangwang'}

18.var.remove('zhangfei')
print(var)
{'h', 'a', 'n', 'e', 'i', 'g', 'z', 'zhangbo', 'zahngfei', 'f', 'zhanglang', 'zhangwang'}

19.anml ={'紫貂','松貂','青鼬','狼獾’}
print(anml,type(anml))

20.with open('avgHgt.csv') as file:
  contents=file.read()
 print(contents)
age,CHeight,JHeight
7,125,122
8,131,128
9,138,133
10,140,138
11,145,143
12,153,153
13,161,155
14,169,162
15,174,166
16,174,169
17,174,170
18,175,171

21.with open('avgHgt.csv') as file:
 lines=file.readlines()
for line in lines:
   print(line.rstrip())
age,CHeight,JHeight
7,125,122
8,131,128
9,138,133
10,140,138
11,145,143
12,153,153
13,161,155
14,169,162
15,174,166
16,174,169
17,174,170
18,175,171

22.import pandas as pd
mydata=pd.read_csv('avgHgt.csv',encoding = 'utf-8')
print(mydata)
    age  CHeight  JHeight
0     7      125      122
1     8      131      128
2     9      138      133
3    10      140      138
4    11      145      143
5    12      153      153
6    13      161      155
7    14      169      162
8    15      174      166
9    16      174      169
10   17      174      170
11   18      175      171

23.mydata1 = pd.read_table('avgHgt.csv')
print(mydata1)
   age,CHeight,JHeight
0            7,125,122
1            8,131,128
2            9,138,133
3           10,140,138
4           11,145,143
5           12,153,153
6           13,161,155
7           14,169,162
8           15,174,166
9           16,174,169
10          17,174,170
11          18,175,171

24. import pandas as pd
data2 = pd.read_csv('avgHgt.csv',sep = '',names=['name'],index_col="name")
print(data2)
Empty DataFrame
Columns: []
Index: [age,CHeight,JHeight, 7,125,122, 8,131,128, 9,138,133, 10,140,138, 11,145,143, 12,153,153, 13,161,155, 14,169,162, 15,174,166, 16,174,169, 17,174,170, 18,175,171]
>>
