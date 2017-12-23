import java.math.BigInteger;
import java.util.*;
import java.io.*;
class Fact3 {

   public static void main(String[] args) {
       Scanner s = new Scanner(System.in);
       int n = s.nextInt();

       for(int i=0;i<n;i++)
       {
       int a = s.nextInt();
       String fact = factorial(a);

       System.out.println(fact);
   }
}
   public static String factorial(int n) {
       BigInteger fact = new BigInteger("1");
       for (int i = 1; i <= n; i++) {
           fact = fact.multiply(new BigInteger(i + ""));
       }
       return fact.toString();
   }
}
