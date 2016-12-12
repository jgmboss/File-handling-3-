import java.io.FileReader;
import java.io.BufferedReader;
import java.io.IOException;


public class Qthree
{
    public static void main (String [] args) throws IOException{
        String arry [][] = new String [5][2];


        FileReader fr = new FileReader("U:\\Computer Science\\stuff.txt");
        BufferedReader br = new BufferedReader(fr);


        for (int r = 0; r < 4; r++){
            String line = br.readLine();
            arry[r][0] = line.substring(0,5);
            arry[r][1] =  line.substring(5);
        }
        br.close();


        System.out.println (arry[0][0]);
    }
}
