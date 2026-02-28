```java
import java.util.*;
 
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
 
        int n = sc.nextInt();
 
        long[] arr = new long[n];
        long min = Long.MAX_VALUE;
        long max = Long.MIN_VALUE;
        for(int i =0;i<n;i++){
            arr[i]=sc.nextLong();
            if(arr[i]<min) min = arr[i];
            if(arr[i]>max) max = arr[i];
        }
        int ans = 0;
        for(int i=0;i<n;i++){
            if(arr[i]<max && arr[i]>min) ans++;
        }
        System.out.println(ans);
 
 
 
 
    }
}
