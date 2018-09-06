# coding:utf-8
# list_tuple_dict
列表、元组、词典之间的转换。

# 1 字典
dict = {'name': 'A', 'age': 24, 'class': 'First'}
	# 1.1 转换为字符串，返回<type 'str'>{'age': 7, ...}
print type(str(dict)), str(dict)
	# 转为元组
print tuple(dict)
	# 字典转为元组返回，（7， A， first）
print tuple(dict.values())
	# 转换为列表，返回[age, name, class]
print list(dict)
	# 转换为列表
print dict.values()
# ------------元组-----------
tup = (1, 2, 3, 4, 5)

	# 转换为字符串,返回：(1, 2, 3, 4, 5)
print tup.__str__()
	# 转为列表，返回[1,2,3,4,5]
print list(tup)
	# 元组不可以转为字典

# 3 列表
nums = [1, 3, 5, 7, 8, 13, 20]
	# 转为元组
print tuple(nums)
	# str
print str(nums)
	# 列表不可以转为字典

# 4 字符串
	# 字符串转为元组
print tuple(eval('(1, 2, 3)'))
	# 转为列表
print list(eval(('1, 2, 3')))
	# 字符串转为字典，返回：<type 'dict'>
print type(eval("{'name':'ljq', 'age':24}"))

