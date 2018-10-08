# Python-
在Python中可以用一些1代表True或则用o代表False吗

先来看段代码:

  li1= [1,0,2,5,6]
  for i in li1:
      if i== True:
          print('为真')
      elif i == False:
          print('为假')
      else:
          print("都不是")
          
这段代码的运行结果是:
    为真
    为假
    都不是
    都不是
    都不是
 
 由此可见,在Python中是可以用数字1代表True或则用o代表False,但是仅限于0和1,类似于C语言里面的逻辑判断.接着
再来看段代码:

      list1= [6,2,7]
    b=True
    for i in range(len(list1)):
        b= b and (list1[i]>5)
    if b == True:
        print('列表list1的结果是：%s' % b)
    else:
        print('列表list1的结果是：%s' % b)
   这段代码的运行结果是:
    列表list1的结果是：False
  
  上述两端代码间接地验证了了我们的想法,结果显示是可行的.第二段代码的作用相当于判断一个列表中的所有数值,是否都
大于一个预设值5,若大于则返回True,否则返回False.其中 b= b and (list1[i]>5) 这句代码里,and的作用就是一个逻辑
比较,只有当两边都为Ture时,才会输出Ture.因此在列表list1中只要有一个数字不符合要求(list1[i]>5),结果就会是False.

待续...

