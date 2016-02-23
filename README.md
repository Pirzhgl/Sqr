import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        double a, b, c, d, x1, x2;
        System.out.println("Введите а: ");
        a = in.nextDouble();
        System.out.println("Введите b: ");
        b = in.nextDouble();
        System.out.println("Введите c: ");
        c = in.nextDouble();
        d = b * b - (4 * a * c);
        if (d > 0) {
            x1 = (-b + Math.sqrt(d)) / (2 * a);
            x2 = (-b - Math.sqrt(d)) / (2 * a);
            System.out.printf("x1 = " + x1 + " x2 = " + x2);
        }
        else if (d == 0){
            x1 = -b / (2 * a);
            System.out.printf("x1, x2 = " + x1);
        }
        else
            System.out.print("Ошибка. D меньше нуля");
        
        
    }

}
