##
python多次接触，很多项目基本都用到了python，但每次对于一些基础的语法和概念，似乎都要从头开始学，这里是根据廖雪峰的python教学网站简要过了一遍，
这里记录了一下本次复习中觉得一些有用且重要的：
##
1.list可变[],tuple不可变()
classmate=["a","b","c"]
tuple=(1,2,3)
list常用法有: 
classmate.append("d") #添加
classmate.insert(1,"e") #插入
classmate.pop() #删除末尾元素
classmate.pop(1) #删除指定位置元素
len(classmate) #获取长度
##
2.I/O 简单输入输出
例子：print('%2d-%02d' % (3, 1))
输出：3-01
例子：print(f'The area of a circle with radius {r} is {s:.2f}')
输出：The area of a circle with radius 2.5 is 19.62
##
3，if else 语句后记得加冒号
例子： if age>=18:
         print('adult')
       elif age<=6:
          print('child')
        else:
        print('teenager')
##
4.新加入的模式匹配 match（了解）
##
5.break结束后续所有循环，continue结束当前循环，继续下一次循环
##
6.dict字典相关，key键一定是不可变元素，用{}表示字典，而set则是一系列键的合集也用{}表示
tuple虽然是不可变对象，但是当其内部包含列表等可变对象如（1,2，[1,2,3]），则其不可用于键
一些用法：
新增字典元素：dict[key]=value
新增set元素：set.add(element)
删除字典元素：dic.pop(key)
删除set元素：set.remove(element)
判断某个元素是否在字典中 ：dict.get("value",-1)
##
7.函数相关
7.1 函数名其实就是指向一个函数对象的引用，完全可以把函数名赋给一个变量，相当于给这个函数起了一个“别名”：
例子：
a=abs #注意这里无括号，因为不是调用
a(-1)
