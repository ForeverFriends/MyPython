# 数组的创建
![](../images/array.png)

    import numpy as np

    arry = np.array([-9,7,4,3])		# 创建数组

    np.arange(0,10,1) 				# 创建[0,10)间隔为1的数组（等差数组）

    np.linspace(0,10,10)			# 创建[0,10]间等差的10个数组成的数组

    np.linspace(0,10,10, endpiont = False)  #创建[0,10]间等差的10个数组成的数组


  #创建等比数列，长度为10，2为底数，指数为1至5之间的10个等差数列  
    
    np.logspace(1, 5, base = 2, num = 10) ==>  array([ 2.,  2.72158,  3.70349885,  5.0396842 ,  6.85795186,
    												9.33223232, 12.69920842, 17.28095582, 23.51575188, 32.])
    #相当于：
    2**np.linspace(1,5,10)

  #创建全0数组：

    np.zeros(4) ==> array([0,0,0,0])

  #创建2行3列全1数组

    np.ones([2,3]) ==>  array([[1., 1., 1.],
       						  [1., 1., 1.]])
    

  #ndim属性 返回维度

    array1 = np.ones([2,3])
    array1.ndim  ==> 2
	arry.ndim ==> 1

  #shape属性 返回行列数

    arry1.shape ==> (2,3)
    #注意shape作用与一维数组返回为列数
    arrry.shape ==> (4,)

  #size 数量

    arry.size ==> 4

  #dtype 数组元素类型

    arry.dtype ==> (int32)