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
 




