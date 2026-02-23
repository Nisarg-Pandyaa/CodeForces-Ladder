```java
import java.util.*;
 
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
 
        int k = sc.nextInt();
 
        int[] month = new int[12];
        int max = -1;
        for(int i=0;i<12;i++){
            month[i] = sc.nextInt();
            if(month[i]>max) max = month[i];
        }
 
        if(k==0){
            System.out.println(0);
            return;
        }
        if(max>=k){
            System.out.println(1);
            return;
        }
        int i=11;
        Arrays.sort(month);
        int months = 0;
        while(k>0){
            k -= month[i];
            i--;
            months++;
            if(i==-1 && k>0){
                System.out.println(-1);
                return;
            }
        }
        System.out.println(months);
    }
}
