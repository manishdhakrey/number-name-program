# number-name-program
import java.util.Scanner;

public class NumberNames {
    public static void main(String[] arg){
        String[] s1={"one","two","three","four","five","six","seven","eight","nine"};
        String[] s2={"eleven","twelve","thirteen","fourteen","fifteen","sixteen","seventeen","eighteen","nineteen"};
        String[] s3={"ten","twenty","thirty","fourty","fifty","sixty","seventy","eighty","ninty","hundred"};
        Scanner scannerobject=new Scanner(System.in);
        System.out.println("Please Enter a Number Between 0 to 100");
        int n=scannerobject.nextInt();
        scannerobject.close();
        if(n%10==0){
            int a=n/10;
            String b=s3[a-1];
            System.out.println(n+"can be written as :"+b);
        }
        else if(n>0 && n<10){
            String b=s1[n-1];
            System.out.println(n+"can be written as :"+b);
        }
        else{
            int a=n/10;
            int b=n%10;
            String x=s3[a-1];
            String y=s1[b-1];
            System.out.println(n+"can be written as :"+x+"-"+y);
        }
    }
}
