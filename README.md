# Java_tasks

#### Из секунд в часы минуты секунды.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = (a/(60*60))%24,
                c=(a/60)%60, d=a%60;
        System.out.format("%02d"+":"+"%02d"+":"+"%02d",b,c,d);

    }
}
```

#### Дни в секунды
```
import java.util.Scanner;
class MyProgram {
	public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print(sc.nextInt() * 24 * 60 * 60);
	}
}
```

#### На вход подаются числа, которые делятся на 11. Концом последовательности будет любое число, не делящееся на 11 (это число не входит в последовательность).

Посчитайте количество введённых чисел и сумму тех из них, которые кратны 3.
```
import java.util.Scanner;

class MyTest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = 0;
        int count = 0, sum = 0;

        while ((a=sc.nextInt()) % 11== 0 ){
                count++;
             if (a% 3 == 0){
                sum+= a;
                a++;
            }
        }

        System.out.println(count);
        System.out.println(sum);
    }
}
```

#### Числа от 0 до 10 если число больше то break.
```
import java.util.Scanner;
class MyTest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double a = 0;
        double count = 0, sum = 0;
        while ((a=sc.nextInt()) >= 0 && a<11){
            count++;sum+= a;
        }
        System.out.println(sum/count);
    }
}
```
#### Отзеркалить String, int.
```
import java.util.Scanner;
class Kol {
    public static void main(String[] args) {
        int q = 465478;
        String p = Integer.toString(q);
       String a = "город доро";
       StringBuilder b = new StringBuilder(p);
       b = b.reverse();
        System.out.println(b.toString());
    }
        }
```

#### на вход подаётся два натуральных числа - n и m. Напечатайте число n, повторённое m раз в одной строке через пробел.
Sample Input:

3 5
Sample Output:

3 3 3 3 3
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = sc.nextInt();
        for (int i = 0; i < b; i++) {
                System.out.print(a+" ");
            }
    }}
```

#### На вход подаётся два натуральных числа x и y. Выведите на печать прямоугольник из звёздочек размером x*y.
Sample Input:

4 2
Sample Output:

**
**
**
**
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a =sc.nextInt(), b = sc.nextInt();
        for (int i = 1; i <= a; i++) {
            System.out.println();
                for (int j = 0; j < b; j ++) {
                    System.out.print("*");
            }
            }
    }}
```

#### лесенка
Напечатайте "лесенку" из чисел от единицы до n, n > 0.

Примечание. Каждая строка в "лесенке" заканчивается цифрой (не пробелом).
```
import java.util.Scanner;

class Example {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        for (int i = 1; i <= a; i++) {
            for (int j = 1; j <= i; j++) {
                if(i==j){
                    System.out.print(j+"\n");
                } else {
                    System.out.print(j+" ");
                }
            }
        }
    }
}
```

#### Двумерный массив
 Два индийских программиста, Махатма и Джавахарлал, вдруг обнаружили, что таблица умножения иногда весьма полезна для программистов, и решили её выучить. Помогите нашим индийским друзьям!

На вход подаются числа n и m. Выведите таблицу умножения n * m (см. пример).

Sample Input:

3 4
Sample Output:

1 2 3 4
2 4 6 8
3 6 9 12

```
import java.util.Scanner;
class Example {
    public static void main(String[] args) {
        Scanner sc =new Scanner(System.in);
        int a =sc.nextInt(), b = sc.nextInt();
        int [][] num = new int[a][b];
        for (int i = 0; i<a; i++) {
            for (int j = 0; j < b; j++) {
                num[i][j] = (i + 1) * (j + 1);
                if (j == b - 1) {
                    System.out.print(num[i][j]);
                } else {
                    System.out.print(num[i][j] + " ");
                }
            }
            System.out.println();
        }
}}
```
#### Матрица
На вход подаётся матрица (двумерный массив). Все элементы матрицы - целые числа. Найдите её размеры и выведите на печать в соответсвии с примером.

Sample Input 1:

1 2 3
4 5 6
7 8 9
Sample Output 1:

Строк: 3
Столбцов: 3
Sample Input 2:

1 2
3 4
5 6
7 8
Sample Output 2:

Строк: 4
Столбцов: 2

```
import java.util.*;
class MySolution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = 0;
        int b = 0;
        while(sc.hasNext()){
            String[] Arr = sc.nextLine().split(" ");
            b = Arr.length;
            a++;
        }
        System.out.println("Строк: "+a);
        System.out.print("Столбцов: "+b);
    }
}
```