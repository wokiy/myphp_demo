# php入门旅途
 > 简介PHP（外文名:PHP: Hypertext Preprocessor，中文名：“超文本预处理器”）是一种通用开源脚本语言。语法吸收了C语言、Java和Perl的特点，利于学习，使用广泛，主要适用于Web开发领域。PHP 独特的语法混合了C、Java、Perl以及PHP自创的语法。它可以比CGI或者Perl更快速地执行动态网页。用PHP做出的动态页面与其他的编程语言相比，PHP是将程序嵌入到HTML（标准通用标记语言下的一个应用）文档中去执行，执行效率比完全生成HTML标记的CGI要高许多；PHP还可以执行编译后代码，编译可以达到加密和优化代码运行，使代码运行更快
 
 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src="http://5b0988e595225.cdn.sohucs.com/images/20171123/83b690046b9d4cf484cceb1b66c9dc14.gif" style="margin-left:25%;"/>
 
#### 入门案例
1. 案例1
 ```
  <?php
   header('content-type:text/html; charset=utf-8');
   $name = 'jasonlwy';
   $age = 24;
   $color = 'red';
   $people = array('name'=>'jasonlwy', 'age'=>24, 'color'=>'red');
  ?>
  ```
2. 案例二（面向对象的写法）
 ```
   <?php
    header('content-type:text/html; charset=utf-8');
    class people{
     public $name;
     public $age;
     public $color;
    }
    $jasonlwy = new people;
    $jasonlwy->name = 'summery';
    $jasonlwy->age = 22;
    $jasonlwy->color = 'red';
    echo $jasonlwy->name.$jasonlwy->age.$jasonlwy->color;
   ?>
   /*
    class关键字 表示一个类，public $name 成员属性 public设置访问权限对应的还有protected private等访问修饰符
    $jasonlwy = new class //实例一个对象
    $jasonlwy->name = 'dd';属性成员赋值 ->对象访问符
    var_dump 输出对象的详细信息
   */
 ```
3. 对象传递方式
 ![](http://114.215.91.58/Blog//static/userImages/20180510/1525920235766047921.png)
 
 ![](http://114.215.91.58/Blog//static/userImages/20180510/1525920235858000796.png)
 
4. 成员方法基本语法
 ```
  class  类名{
     成员属性;
    访问修饰符  function  成员方法1名(形参){
        方法体;
       return 语句;//[是有程序员自己决定的,]
    }
        访问修饰符  function  成员方法1名(形参){
        方法体;
      return 语句;//
     }
   }
   /* 
    (1)	成员方法定义在类中.
    (2)	成员方法前面可以有访问修饰符，如果你不写，默认为public
    (3)	成员方法的运行原理和普通的函数是一样的
   */
  ```

 
 
