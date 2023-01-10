## 1.10日Java学习
1.数据类型相关(Java是强类型语言)

      基本类型：byte,short,int,long,float,double,char,boolean

      引用类型：类(String属于这一类)，接口（interface），数组

2.转义字符

      \n换行

      \t对齐

      \\输出\

      \"输出"

      \r不同的编辑器效果不同
 
3.类型转换
      
      强制类型转换：高->低，可能会损失精度，甚至有可能内存溢出
      ```
      int i=128;
      byte b=(byte)i;
      ```
      自动转换：低->高
      ```Java
      int i=10;
      double b=i;//不用（double）了
      ```
      注意事项：不要对boolean进行转换
4.变量

      Type Name[=value]{[,Name2=value]};

      局部变量：
            例子：int a=10;
            
      实例变量：方法外面，类里面，不用非要初始化,会有默认值，注意boolean的默认值是false
            例子1：String name;//若不初始化，默认为null
            例子2：Demo demo1=new Demo();//也是实例变量，其中Demo就是class Demo{...}所定义的

      类变量：加了static关键字的，好处是不用new一个对象
      
5.常量
      
      final 常量名=值；
      常量名一般用大写
      例子：final double PI=3.1415;
 
6.规范

      可以去看阿里巴巴的Java开发手册

      
      
      
      

      
