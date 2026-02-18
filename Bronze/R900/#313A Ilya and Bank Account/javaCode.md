```java
import java.util.*;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
 
        long n = sc.nextLong();
 
        if(n>=0){
            System.out.println(n);
            return;
        }
 
        long removeLastDigit = n/10;
        long lastDigit = n%10;
        long remove2ndLastDigit = (n/100);
        remove2ndLastDigit *= 10;
        remove2ndLastDigit += lastDigit;
 
        if(removeLastDigit >= remove2ndLastDigit) System.out.println(removeLastDigit);
        else System.out.println(remove2ndLastDigit);
    }
 
 
}
