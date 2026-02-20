```java
import java.util.*;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int m = sc.nextInt();

        int ans = 0;
        ans = n;

        while(n >= m){

            ans += (n/m);
            int x = n%m;
            n /= m;
            n += x;

        }
        System.out.println(ans);


    }
}
