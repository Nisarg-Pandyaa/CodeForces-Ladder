```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Byte n = sc.nextByte();
        Byte m = sc.nextByte();

        int[] arr = new int[n];

        for(int i=0;i<n;i++){
            arr[i] = sc.nextInt();
        }

        Arrays.sort(arr);
        int maxMoney = 0;

        for(int i=0;i<m;i++){
            if(arr[i]<0){
                maxMoney += Math.abs(arr[i]);
            }
            if(arr[i]>=0) break;
        }

        System.out.println(maxMoney);
    }
}

  
  
