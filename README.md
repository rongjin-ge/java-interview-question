# java-interview-question

一、String,StringBuffer, StringBuilder 的区别是什么？String为什么是不可变的？  
答：  
1、String是字符串常量，StringBuffer和StringBuilder都是字符串变量。后两者的字符内容可变，而前者创建后内容不可变。  
2、String不可变是因为String对象内部的char[]是private的,并且没有提供setValue方法,所以在String类的外部无法修改String。  
3、StringBuffer是线程安全的(底层采用synchronized)，而StringBuilder是非线程安全的。  
ps：线程安全会带来额外的系统开销，所以StringBuilder的效率比StringBuffer高。  

