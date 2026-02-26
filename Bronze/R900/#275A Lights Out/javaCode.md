```java
import java.util.*;
public class Main {
 
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
 
        int[][] grid = new int[3][3];
        int[][] lights = new int[3][3];
 
        for(int i=0;i<3;i++){
            for(int j=0;j<3;j++){
                grid[i][j] = sc.nextInt();
            }
        }
 
        Arrays.fill(lights[0],1);
        Arrays.fill(lights[1],1);
        Arrays.fill(lights[2],1);
 
        if(grid[0][0]%2!=0){
            lights[0][0] = (lights[0][0]==1) ? 0 : 1;
            lights[0][1] = (lights[0][1]==1) ? 0 : 1;
 
            lights[1][0] = (lights[1][0]==1) ? 0 : 1;
        }
        if (grid[0][1]%2!=0) {
            lights[0][1] = (lights[0][1]==1) ? 0 : 1;
 
            lights[0][0] = (lights[0][0]==1) ? 0 : 1;
            lights[1][1] = (lights[1][1]==1) ? 0 : 1;
 
            lights[0][2] = (lights[0][2]==1) ? 0 : 1;
 
        }
        if(grid[0][2]%2!=0){
            lights[0][2] = (lights[0][2]==1) ? 0 : 1;
            lights[0][1] = (lights[0][1]==1) ? 0 : 1;
 
            lights[1][2] = (lights[1][2]==1) ? 0 : 1;
        }
        if(grid[1][0]%2!=0){
            lights[1][0] = (lights[1][0]==1) ? 0 : 1;
            lights[0][0] = (lights[0][0]==1) ? 0 : 1;
 
            lights[1][1] = (lights[1][1]==1) ? 0 : 1;
 
            lights[2][0] = (lights[2][0]==1) ? 0 : 1;
        }
        if(grid[1][1]%2!=0){
            lights[1][1] = (lights[1][1]==1) ? 0 : 1;
 
            lights[0][1] = (lights[0][1]==1) ? 0 : 1;
 
            lights[1][0] = (lights[1][0]==1) ? 0 : 1;
            lights[1][2] = (lights[1][2]==1) ? 0 : 1;
 
            lights[2][1] = (lights[2][1]==1) ? 0 : 1;
 
        }
        if(grid[1][2]%2!=0){
            lights[1][2] = (lights[1][2]==1) ? 0 : 1;
            lights[0][2] = (lights[0][2]==1) ? 0 : 1;
 
            lights[1][1] = (lights[1][1]==1) ? 0 : 1;
 
            lights[2][2] = (lights[2][2]==1) ? 0 : 1;
        }
        if(grid[2][0]%2!=0){
            lights[2][0] = (lights[2][0]==1) ? 0 : 1;
            lights[1][0] = (lights[1][0]==1) ? 0 : 1;
 
            lights[2][1] = (lights[2][1]==1) ? 0 : 1;
        }
        if(grid[2][1]%2!=0){
            lights[2][1] = (lights[2][1]==1) ? 0 : 1;
            lights[2][0] = (lights[2][0]==1) ? 0 : 1;
 
            lights[1][1] = (lights[1][1]==1) ? 0 : 1;
 
            lights[2][2] = (lights[2][2]==1) ? 0 : 1;
        }
        if(grid[2][2]%2!=0){
            lights[2][2] = (lights[2][2]==1) ? 0 : 1;
            lights[1][2] = (lights[1][2]==1) ? 0 : 1;
 
            lights[2][1] = (lights[2][1]==1) ? 0 : 1;
        }
 
        for(int i=0;i<3;i++){
            for(int j=0;j<3;j++){
                System.out.print(lights[i][j]);
            }
            System.out.println();
        }
    }
 
 
}
