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