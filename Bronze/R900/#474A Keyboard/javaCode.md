```java
import java.util.*;

 public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        char c = sc.next().charAt(0);
 
        String s = sc.next();
 
        StringBuilder sb = new StringBuilder();
        String keybord = "qwertyuiop" +
                "asdfghjkl;" +
                "zxcvbnm,./";
        int n = s.length();
 
        if(c=='L'){
            for(int i=0;i<n;i++){
                sb.append(keybord.charAt(keybord.indexOf(s.charAt(i))+1));
            }
        }else{
            for(int i=0;i<n;i++){
                sb.append(keybord.charAt(keybord.indexOf(s.charAt(i))-1));
            }
        }
        System.out.println(sb);
    }
}
