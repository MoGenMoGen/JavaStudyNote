<h1 style="text-align:center">java杂项内容 </h1>

> 这里主要放置一些比较杂，不方便归类的知识点

+ JDK、JRE、JVM的关系

```js
JDK=JRE+java开发工具
JRE=JVM+核心类库
```

+ 环境变量path配置及其作用

```js
1.为了可以在dos的任意目录使用javac和java命令
2.先配置 JAVA_HOME=JDK安装主目录
3.%JAVA_HOME%\bin 引用JAVA_HOME路径
```

		+ 获取数据类型

```java
//定义
public static String getType(Object o){
        return o.getClass().toString(); //使用int类型的getClass()方法
    }
//调用
  System.out.println(getType(a));

```

+ java中''只能放字符，""存字符串