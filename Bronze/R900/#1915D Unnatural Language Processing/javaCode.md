```java
import java.util.*;
 
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
 
        int t = sc.nextInt();
 
 
 
        while(t-- > 0) {
            int n = sc.nextInt();
            String s = sc.next();
            int i=n-1;
 
            List<String> al = new ArrayList<>();
 
            while(i>=0){
                String res;
                if(s.charAt(i)=='a' || s.charAt(i)=='e'){
                    res = s.substring(i - 1, i + 1);
                    i -= 2;
                }
                else{
                    res = s.substring(i-2,i+1);
                    i -= 3;
 
                }
                al.addFirst(res);
            }
 
            int l = al.size();
            i = 0;
            while(i<l){
                System.out.print(al.get(i));
                if(i!=l-1) System.out.print('.');
                i++;
 
            }
            System.out.println();
 
 
        }
    }
}
