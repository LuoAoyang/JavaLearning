## day03---1.13日所学内容

1.选择结构

    if选择结构：
    a.if(表达式){
    ...
    }
    b.if(表达式){
    ...
    }else{
    ...
    }
    c.if(表达式){
    ...
    }else if{
    ...
    }else if{
    ...
    }else{
    ...
    }
    
    switch选择结构：
    switch(表达式){
      case 值：
      ...;
      break;
      case 值：
      ...;
      break;
      ...
      default:
    }
    switch 语句中的变量类型可以是： byte、short、int 或者 char。从 Java SE 7 开始，switch 支持 String 类型了，同时 case 标签必须为字符串常量或字面量。
    break有或者没有，语句的意思可能完全不一样。

2.循环结构：

    while循环，do...while循环，for循环
    while(){
    ...
    }
    
    do{
    ...
    }while();
    
    for( ; ; ){
    ...
    }
    for循环增强：
    例子：int[] num={1,2,3,4,5};
    for(int x:num){
    System.ou.println(x);
    }
    
    break,continue,goto(注：Java中没有goto，但又他的思想)
    break:跳出循环，通俗的说跳出一个大括号
    continue：跳出当前训话，例如此处不能等于5，使用continue跳出i=5的情况，但是i=6,7...的情况还是会有
    goto:尽管goto仍是Java的一个保留字，但并未在语言中得到正式使用。在Java中可以用标签label,举例(注意outer和continue outer;)：
    
    public class Demo {
    public static void main(String[] args) {
        //打印101-150之间所有的质数
        //质数是指在大于1的自然数中，除1和它本身以外不再有其他因数的自然数
        int count = 0;

        outer:for (int i =101;i<150;i++){
            for (int j = 2;j<i;j++){
                if (i % j == 0){
                    continue outer;
                }
            }
            System.out.print(i+"  ");
        }
    }
    
3.方法

        方法：修饰符 返回值类型 方法名(变量类型 变量名，...){
        ...
        return 返回值;
        }
        返回值类型为空，用void
        方法重载：一个类的两个方法具有相同的名字，方法重载返回值类型可以相同或者不相同，
        但变量类型它的类型或者顺序必须不同，即参数列表必须不同，所以只根据返回值类型不同无法判断这个重载是否有效
        命令行传参：(但现在我不太明白具体有什么用，或者应该用到哪里)
        例子：
        package com.luoaoyang.study;
        //命令行传参
        public class Demo02 {
        public static void main(String[] args) {
            for(int i=0;i< args.length;i++){
                System.out.println(args[i]);
                }
            }
        }
        可变参数：1个方法中只能有一个可变参数，且必须在最后
        格式为typeName... parameterName
        例子：void(int... a)、double(double... num)
        递归讲解：程序调用自身，调用的本质就是栈的先进后出，不过递归一般不适用，因为递归太多次占用的空间内存也很大，电脑受不住
        
4.数组

        数组的定义：int[] a=new int[10];
        java中也有类似与c、c++的int a[];但我们一般使用上面的
        
        
        
 




