import java.util.Scanner;
public class Main {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);
        System.out.print("Kaç Sayi Gireceksiniz: ");
        int sayi = input.nextInt();
        int max = 0,min = 0;
        for(int i=1; i<=sayi; i++){
            System.out.print(i+".sayiyi giriniz: ");
            int sayilar = input.nextInt();

            if(i==1){
                max=sayilar;
                min=sayilar;
            }
            else{
                if(sayilar>max){
                    max=sayilar;
                }
                else if(sayilar<min){
                    min = sayilar;
                }
            }
        }
        System.out.println("Max:"+max);
        System.out.println("Min"+min);






    }
}
