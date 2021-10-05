<h1 style="text-align:center;">java基础</h1>

### 数据类型转换

```java
1.int->String
    int a=2;

1.1	String b=a+""；
1.2 String s=String.valueOf(i);

 2.String->int
String s="12345";
int i;
第一种方法：i=Integer.parseInt(s);
第二种方法：i=Integer.valueOf(s).intValue();
String转其他类型类似
    例如String->double
    double i=Double.parseDouble	(s);
```

### 猜数字游戏

> 一、Scanner类，获取输入值
>
> 1.导入Scanner包；2.创建Scanner对象；3.next()代表字符串，类似的还有nextInt()、nextDouble()；
>
> 二、Random生成随机数
>
> 1.导入Random包；2.创建Random对象；3.nextInt()、nextDouble()生成对应类型的随机数；

```java
import com.sun.org.apache.xpath.internal.objects.XString;

import java.util.Random;
import java.util.Scanner;

public class test01 {
    public static void main(String[] args) {
        //猜数字游戏
        //创建Scanner对象
        Scanner myScanner = new Scanner(System.in);
//        生成随机数
            Random r = new Random();
        int target = r.nextInt(99) + 1; // 生成[1,100]区间的整数
        int temp = 0;
        System.out.print("请输入一个数字:");
        temp = myScanner.nextInt();

        while (temp != target) {

            if (temp > target) {
                System.out.print("请输入一个小一点的数字:");
                temp = myScanner.nextInt();
            } else if (temp < target) {
                System.out.print("请输入一个大一点的数字:");
                temp = myScanner.nextInt();
            } else
                break;

        }
        if (temp == target)
            System.out.print("恭喜你，回答正确！");

    }
  
}


```

