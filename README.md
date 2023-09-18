# L_02_Z2_Matraeva
import java.util.Scanner;

public class NumberMatrix {
    public static void main(String[] args){
        Scanner scanner = new Scanner(System.in);
        System.out.print("Введiть значення N: ");
        int n = scanner.nextInt();
        int k = n*n;
        int [][] matrix = new int [n][n];
        int num = 1; //Початкове число для заповнення матриці
        for (int i=0; i < n; i++) {
        for (int j=0; j < n; j++){
            matrix[i][j] = num;
            num++;
        }
        }
        //Виведення матриці на екран
        for(int i = 0; i < n; i++){
            for(int j = 0; j < n; j++){
                System.out.print(matrix[i][j] + "\t");
            }
            System.out.println();
        }
        scanner.close();
    }
    }
