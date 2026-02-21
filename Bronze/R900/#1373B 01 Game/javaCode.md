```java
import java.util.*;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
 
        int t = sc.nextInt();
 
        while(t-- > 0){
            StringBuilder sb = new StringBuilder(sc.next());
            int moves = 0;
            while(sb.indexOf("01")!=-1 || sb.indexOf("10")!=-1){
                if(sb.indexOf("01")!=-1){
                    sb.delete(sb.indexOf("01"),sb.indexOf("01")+2);
                    moves++;
                }
                if(sb.indexOf("10")!=-1){
                    sb.delete(sb.indexOf("10"),sb.indexOf("10")+2);
                    moves++;
                }
            }
 
            if(moves%2==0) System.out.println("NET");
            else System.out.println("DA");
        }
    }
}
