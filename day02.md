## 1.11第二天的学习

1.各种运算符：

    一元运算符：++，--自增，自减运算...

    二元运算符：+，-，*，/,%...

    三元运算符：x？y:z

2.位运算符
    
    &:位与
    |:位或
    ^:异或
    ~:取反
    >>:右移
    <<:左移
    注意都是在二进制下的
 
3.逻辑运算符

    &&：与
    ||：或
    ！：非
    
4.包

    package
    例子：package com.baidu.www
    导入包：
    例子：import java.util.Scanner 

5.Javadoc

    文档注释相关的内容
    有@author
      @since
      @version
      @param
      @return
      @throws
      Javadoc可以生成一个文件夹，里面存放有关于类的详细信息
      
6.Scanner

    记得在程序前面加上import java.util.Scanner 
    使用
    例子：Scanner scanner = new Scanner(System.in);
        String str=scanner.nextLine();
        System.out.println(str);

7.顺序结构

    最简单的结构，程序自上而下进行
