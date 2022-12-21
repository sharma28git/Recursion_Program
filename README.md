# Recursion Program of DSA
Fibonacci Series Program :
#Program simple approach:
import java.util.Scanner;
public class MyClass {
    public static void main(String args[]){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int a=0, b=1, c;
        for(int i=0;i<=n;i++){
            System.out.print(a+" ");
            c=a+b;
            a=b;
            b=c;
    }
}
}

#Program by Recursion method:

import java.util.Scanner;
public class MyClass {
    static int Fibonacci(int n){
        if(n <= 1){
            return n;
        }
        else{
            return Fibonacci(n-1)+Fibonacci(n-2);
        }
    }
    public static void main(String args[]){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        for(int i=0;i<=n;i++){
            System.out.print(Fibonacci(i)+" ");
        }
}
}

--------------------------------------------------------

# Factorial Program by Recursion:
import java.util.Scanner;
public class MyClass {
    static int fact(int n){
        if(n == 0){
            return 1;
        }
        else if(n == 1){
            return 1;
        }
        else{
            return n*fact(n-1);
        }
    }
    public static void main(String args[]){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        System.out.print("Factorial is:"+" "+fact(n));
        
}
}

